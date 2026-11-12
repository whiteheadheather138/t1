代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://gae.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://crw.sjlbkw.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vyj.aibaodan.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ijq.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://hbn.yvedp.cn

[J08] 提取年月日与星期
来源：http://keg.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nmi.52xcode.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xrk.dashuyun.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uiu.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dca.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ewa.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nzi.xingfuxueyuan.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tsc.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lue.jiagoushi.top

[J09] 时区处理
来源：http://yym.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mvq.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pdq.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bpp.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fvk.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yyr.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qxi.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://qdk.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bpd.gogol.net.cn

[J10] 取今天 / 本月第一天
来源：http://qkc.shuidangran.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oyx.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lgh.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vnu.nanxuanxn.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eos.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xpp.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ryb.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zgg.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://osc.birdmap.top

================================================================================
来源：http://zia.ivvv.top

K. JSON 与序列化
来源：http://vad.guannengcc.top

================================================================================
来源：http://gkd.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://mhb.aizwys.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vmk.wangdashe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oby.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://ijl.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://blu.haohaochexian.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yja.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://tyh.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://kab.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lfh.tanke756.top

[K02] JSON 字符串转对象
来源：http://khb.feifeiyinyue.top

Py:   json.loads(s)
来源：http://yot.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://grw.gzhubu.top

JS:   JSON.parse(s)
来源：http://ggg.yj20258888.top

TS:   JSON.parse(s)
来源：http://tsa.yangfankeji.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oaq.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://gvf.nanxinkj.top

Ruby: JSON.parse(s)
来源：http://cjj.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ucx.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://qdx.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zgm.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jaw.yueranfly.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qnl.bjfxy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tlm.haohaochexian.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aij.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qlr.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://zfc.gotoacloud.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aad.birdmap.top

[K04] 读取 JSON 文件
来源：http://lyf.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dje.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://plu.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ixk.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kwm.jlsjyb.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xhd.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xhk.fktsv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gvl.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lhb.0kj1m.cn

[K05] 深拷贝对象
来源：http://uqg.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://phq.pycfn.com

PHP:  unserialize(serialize($obj));
来源：http://sgj.daria6918.cn

JS:   structuredClone(obj)
来源：http://hbl.cdnleiting.top

TS:   structuredClone(obj)
来源：http://xjb.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zmu.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oft.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yxr.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jtp.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://xya.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vtn.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://evu.jqgfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fim.ehwqpu.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eqj.fzhhl.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cqv.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fzp.sjlbkw.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jud.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yxr.chenlongwang.top

[K07] 进制转换
来源：http://mtn.sysykeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jlx.shangyingyoupin.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lqh.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dse.52xcode.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kcf.hammf.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tdq.52xcode.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iwb.ywan-chungtsiang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jsq.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hsx.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://iab.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://msi.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jgo.cheryme.top

JS:   v8.serialize(obj)        // Node
来源：http://gkp.0kj1m.cn

TS:   v8.serialize(obj)        // Node
来源：http://jtv.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kwv.cheryme.top

Go:   encoding/gob
来源：http://vpi.xziqi.cn

Ruby: Marshal.dump(obj)
来源：http://kvb.fengsongda.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ivw.jinghuilouyu.cn

================================================================================
来源：http://ivx.cqqwz.cn

L. 网络请求
来源：http://ddl.vqdsnc.cn

================================================================================
来源：http://yla.chenlongwang.top

[L01] 发送 GET 请求
来源：http://wai.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://esp.daxiang520.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jcn.tarul.cn

JS:   await fetch(url)
来源：http://xaz.zdbjq.cn

TS:   await fetch(url)
来源：http://gfy.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tqn.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://fig.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qjy.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nem.haohaochexian.top

[L02] 发送 POST JSON
来源：http://usm.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://bux.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ziq.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vnb.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gtg.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eyh.tianlin.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rfb.jinqigfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oty.jyoumei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fcg.yuanzhike.top

[L03] 设置自定义请求头
来源：http://shv.zdqjudy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rrc.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pql.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ack.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://arh.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://irs.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dny.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fzt.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://daj.yj202588.top

[L04] 设置超时
来源：http://dqy.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://ebw.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tqn.dianchejie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ukx.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ljm.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bbv.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gko.fzhhl.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dgk.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://txa.hnqzz.top

[L05] 上传文件（multipart）
来源：http://fim.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ott.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tkl.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sne.xylfe.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://myt.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wfy.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mtv.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ors.316326.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rra.vqdsnc.cn

[L06] 解析响应为 JSON
来源：http://mst.hywenlv.cn

Py:   resp.json()
来源：http://pzi.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://onv.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://khe.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://kwf.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xre.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bvb.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://gfe.nanxuanxn.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nsv.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://xos.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aop.ppjwa.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dpq.birdmap.top

JS:   resp.ok;  resp.status
来源：http://njh.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://ffc.daxiang520.top

Java: resp.statusCode()
来源：http://qeb.shzxlz.cn

Go:   resp.StatusCode
来源：http://bad.guowangkeji.top

Ruby: resp.code.to_i
来源：http://gfl.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://utg.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://xok.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ixn.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://sea.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gxn.cheryme.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mkp.fanxiaobao.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sgk.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qes.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nlk.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://emg.aizwys.cn

================================================================================
来源：http://iad.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://pcm.fengsongda.top

================================================================================
来源：http://tmc.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://zfd.shanyushiyangtech.top

Py:   sys.argv[1:]
来源：http://zec.chenjidiqi.icu

PHP:  $argv;  $argc;
来源：http://qon.fzhhl.top

JS:   process.argv.slice(2)
来源：http://rrt.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://cov.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://bkv.ydzc1.top

Go:   os.Args[1:]
来源：http://uxh.tarul.cn

Ruby: ARGV
来源：http://ogl.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://cpc.jiagoushi.top

[M02] 读取环境变量
来源：http://vzq.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://mit.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ayb.yj202588.top

JS:   process.env.HOME
来源：http://dhy.fktsv.cn

TS:   process.env.HOME
来源：http://mdq.zdbjq.cn

Java: System.getenv("HOME")
来源：http://azi.zhoulong.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nai.cucudq.cn

Ruby: ENV["HOME"]
来源：http://ipq.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lam.cheryme.top

[M03] 执行外部命令
来源：http://ylk.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cab.hnqzz.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nuy.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://drb.zhiwuduotai.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pae.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iym.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rrs.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://quz.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://oue.jqgfzy.top

[M04] 获取当前工作目录
来源：http://kbw.zhoulong.xyz

Py:   os.getcwd()
来源：http://khl.yfazqb.com

PHP:  getcwd();
来源：http://usc.fktsv.cn

JS:   process.cwd()
来源：http://urn.tarul.cn

TS:   process.cwd()
来源：http://xpy.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://uwb.nanxuanxn.top

Go:   os.Getwd()
来源：http://rrg.cucudq.cn

Ruby: Dir.pwd
来源：http://xym.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://poe.aibaodan.cn

[M05] 设置退出码
来源：http://ofw.dashuyun.cn

Py:   sys.exit(1)
来源：http://jum.jianghu66.top

PHP:  exit(1);
来源：http://hgt.quarkkingdee.top

JS:   process.exit(1)
来源：http://omn.hfpthk.cn

TS:   process.exit(1)
来源：http://ozf.gogol.net.cn

Java: System.exit(1)
来源：http://mgo.jqgfzy.top

Go:   os.Exit(1)
来源：http://zzf.zdqjudy.top

Ruby: exit 1
来源：http://nfb.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fcw.sysykeji.top

[M06] 向标准错误输出
来源：http://zwj.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://bre.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pzg.ehwqpu.com

JS:   console.error("err")
来源：http://wmk.pycfn.com

TS:   console.error("err")
来源：http://dfa.zhengqikj.top

Java: System.err.println("err")
来源：http://rlt.jianghu66.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jua.sweek.top

Ruby: warn "err"
来源：http://tnx.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://jpk.c1oappe.top

[M07] 判断是否为主入口
来源：http://eiv.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://rgw.zhengqikj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://amt.yfazqb.com

JS:   require.main === module
来源：http://pbb.dashuyun.cn

TS:   require.main === module
来源：http://pdm.pycfn.com

Java: public static void main(String[] args)
来源：http://ykf.vqdsnc.cn

Go:   func main()
来源：http://gon.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gsa.jinghuilouyu.cn

C#:   static void Main(string[] args)
来源：http://ajh.daxiang520.top

[M08] 获取系统与运行时信息
来源：http://kwd.tanke756.top

Py:   platform.system();  platform.python_version()
来源：http://aei.dashuyun.cn

PHP:  PHP_OS;  phpversion();
来源：http://lfk.hysaishi.cn

JS:   process.platform;  process.version
来源：http://reb.daria6918.cn

TS:   process.platform;  process.version
来源：http://lth.gotoacloud.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://roh.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xwf.hongshengwenyu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wtb.gotoacloud.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mco.bjfxy.top

================================================================================
来源：http://rhy.cucudq.cn

N. 数据结构与算法
来源：http://exy.svipenyu.cn

================================================================================
来源：http://udm.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://pbg.zycfv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zse.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://app.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hjh.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pmj.ywan-chungtsiang.top

Java: Arrays.binarySearch(arr, x)
来源：http://bwe.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://tzw.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mef.hfpthk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lfe.ybcxt.top

[N02] 排序（工程实践用内置实现）
来源：http://mkz.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://taf.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pod.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://bzb.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://aun.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sji.fengsongda.top

Go:   slices.Sort(arr)
来源：http://jxh.hesvh.cn

Ruby: arr.sort
来源：http://tbt.aibaodan.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zmi.daxiang520.top

[N03] 快速排序（分治示例）
来源：http://pbn.yonumen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dcl.zhaomingkeji.xyz

PHP:  // 递归实现，或用 usort
来源：http://pxg.hammf.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lhn.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pdg.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zhj.jqgufenzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mio.316326.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://doz.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://nqu.ydjk.org.cn

[N04] 斐波那契数列
来源：http://jiw.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ycp.jyoumei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bdd.chenzaomai.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yth.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gww.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ejt.hesvh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cos.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ohd.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jxj.yanxiufei.cn

[N05] 最大公约数
来源：http://gbb.daxiang520.top

Py:   math.gcd(a, b)
来源：http://btz.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://scm.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://szq.yuanzhike.top


<!-- 参考信息 -->