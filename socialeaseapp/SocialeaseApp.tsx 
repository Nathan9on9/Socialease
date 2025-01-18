import { Button } from "@/components/ui/button"
import { Card, CardContent, CardDescription, CardHeader, CardTitle } from "@/components/ui/card"
import { Tabs, TabsContent, TabsList, TabsTrigger } from "@/components/ui/tabs"
import { Badge } from "@/components/ui/badge"
import { Avatar, AvatarFallback, AvatarImage } from "@/components/ui/avatar"
import { Users, Coffee, Heart, MessageCircle } from 'lucide-react'

export default function SocialeaseApp() {
  return (
    <div className="container mx-auto p-4">
      <h1 className="text-4xl font-bold mb-6 text-center">Socialease</h1>
      <Tabs defaultValue="profile" className="w-full">
        <TabsList className="grid w-full grid-cols-4">
          <TabsTrigger value="profile">Profile</TabsTrigger>
          <TabsTrigger value="matches">Matches</TabsTrigger>
          <TabsTrigger value="practice">Practice</TabsTrigger>
          <TabsTrigger value="chat">Chat</TabsTrigger>
        </TabsList>
        <TabsContent value="profile">
          <Card>
            <CardHeader>
              <CardTitle>Your Profile</CardTitle>
              <CardDescription>Select your interests and take personality tests</CardDescription>
            </CardHeader>
            <CardContent>
              <h3 className="text-lg font-semibold mb-2">Interests</h3>
              <div className="flex flex-wrap gap-2 mb-4">
                <Badge>Computer Science</Badge>
                <Badge>AI</Badge>
                <Badge>Social Skills</Badge>
                <Badge variant="outline">+ Add Interest</Badge>
              </div>
              <h3 className="text-lg font-semibold mb-2">Personality Tests</h3>
              <Button className="w-full mb-2">Take MBTI Test</Button>
              <Button className="w-full">Take Big Five Personality Test</Button>
            </CardContent>
          </Card>
        </TabsContent>
        <TabsContent value="matches">
          <Card>
            <CardHeader>
              <CardTitle>Your Matches</CardTitle>
              <CardDescription>People with similar interests and perspectives</CardDescription>
            </CardHeader>
            <CardContent>
              <div className="grid gap-4">
                {[1, 2, 3].map((user) => (
                  <div key={user} className="flex items-center space-x-4">
                    <Avatar>
                      <AvatarImage src={`https://i.pravatar.cc/150?img=${user}`} alt={`User ${user}`} />
                      <AvatarFallback>U{user}</AvatarFallback>
                    </Avatar>
                    <div className="flex-1">
                      <p className="text-sm font-medium">User {user}</p>
                      <p className="text-sm text-muted-foreground">Interests: Computer Science, AI</p>
                    </div>
                    <Button size="sm">Connect</Button>
                  </div>
                ))}
              </div>
            </CardContent>
          </Card>
        </TabsContent>
        <TabsContent value="practice">
          <Card>
            <CardHeader>
              <CardTitle>Practice Social Skills</CardTitle>
              <CardDescription>Choose a scenario to practice</CardDescription>
            </CardHeader>
            <CardContent>
              <div className="grid gap-4">
                <Button className="justify-start"><Coffee className="mr-2 h-4 w-4" /> Buying Coffee</Button>
                <Button className="justify-start"><Heart className="mr-2 h-4 w-4" /> Approaching Your Crush</Button>
                <Button className="justify-start"><Users className="mr-2 h-4 w-4" /> Introducing Yourself</Button>
              </div>
            </CardContent>
          </Card>
        </TabsContent>
        <TabsContent value="chat">
          <Card>
            <CardHeader>
              <CardTitle>Chat</CardTitle>
              <CardDescription>Talk with your matches or practice with AI</CardDescription>
            </CardHeader>
            <CardContent>
              <div className="grid gap-4">
                <Button className="justify-start"><MessageCircle className="mr-2 h-4 w-4" /> Chat with AI Coach</Button>
                <Button className="justify-start"><Users className="mr-2 h-4 w-4" /> Chat with Matches</Button>
              </div>
            </CardContent>
          </Card>
        </TabsContent>
      </Tabs>
    </div>
  )
}

