代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://ekh.smart0.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wtv.yanxiufei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ogp.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pcl.sufxvd.cn

C#:   d1 < d2;  d1 == d2
来源：http://oku.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://csl.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zgq.cdnleiting.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ydu.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eax.jinghuilouyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nmb.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dci.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bwq.xingfuxueyuan.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ebo.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eva.9152youxi.cn

[J09] 时区处理
来源：http://jjg.shanyushiyangtech.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uiz.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eif.gotoacloud.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qup.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rju.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pmr.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dmc.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dca.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qss.yuxming.cn

[J10] 取今天 / 本月第一天
来源：http://asc.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://otv.yueranfly.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yep.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://erl.xingfuxueyuan.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://scv.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ijt.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://opw.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tkx.nanxuanxn.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iuu.yuxming.cn

================================================================================
来源：http://olk.xziqi.cn

K. JSON 与序列化
来源：http://tmf.hywenlv.cn

================================================================================
来源：http://igv.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://rda.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hge.kuanghao11.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xzc.52xcode.cn

JS:   JSON.stringify(obj)
来源：http://feo.jinyuanbaomall.cn

TS:   JSON.stringify(obj)
来源：http://dyc.9152youxi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tql.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://bob.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://qld.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fam.epnwcf.com

[K02] JSON 字符串转对象
来源：http://rxo.nanxinkj.top

Py:   json.loads(s)
来源：http://lbr.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pnj.yj20258888.top

JS:   JSON.parse(s)
来源：http://tcr.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://cly.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jiy.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://brj.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://nvf.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ypr.andypj.xyz

[K03] JSON 美化输出（带缩进）
来源：http://jpl.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ama.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yqo.xylfe.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bmh.vehdjk.com

TS:   JSON.stringify(obj, null, 2)
来源：http://kol.gotoacloud.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uak.havefunace.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hej.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://ojj.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nqe.tanke756.top

[K04] 读取 JSON 文件
来源：http://pjo.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bxg.cheryme.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vxc.hnxiangtu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hsk.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gdk.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dno.wangdashe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fze.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fzz.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uje.9152youxi.cn

[K05] 深拷贝对象
来源：http://vcz.zdbjq.cn

Py:   copy.deepcopy(obj)
来源：http://bbk.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://ybl.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://wkk.smart0.xyz

TS:   structuredClone(obj)
来源：http://rfz.quarkkingdee.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dyj.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dtp.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://doi.cashguo.top

C#:   // 序列化往返，或自定义 Clone
来源：http://osg.fzhhl.top

[K06] 解析 URL 查询串
来源：http://zrp.yvedp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hkn.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hyx.guannengcc.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tez.ywan-chungtsiang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ijl.yvedp.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ggl.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://plc.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kwk.wangdashe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cxc.fengsongda.top

[K07] 进制转换
来源：http://niw.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mzq.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kmj.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sjs.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bwh.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tcy.havefunace.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ult.fengsongda.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bal.vqdsnc.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://agi.gaohongyu789.top

[K08] 二进制序列化（非 JSON）
来源：http://aly.zdqjudy.top

Py:   pickle.dumps(obj)
来源：http://sir.jqgfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://myq.zhaomingkeji.xyz

JS:   v8.serialize(obj)        // Node
来源：http://wuf.shangyingyoupin.top

TS:   v8.serialize(obj)        // Node
来源：http://pea.hesvh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vxo.iojbl.cn

Go:   encoding/gob
来源：http://bvj.zhiwuduotai.top

Ruby: Marshal.dump(obj)
来源：http://dbb.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ckq.cqqwz.cn

================================================================================
来源：http://lxj.hcnkem.com

L. 网络请求
来源：http://jme.cheryme.top

================================================================================
来源：http://zrg.c1oappe.top

[L01] 发送 GET 请求
来源：http://gmh.havefunace.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tgw.epnwcf.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vmf.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://erj.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://tee.ctjpmb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ntw.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://bhx.fzhhl.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fxl.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://trr.chenlongwang.top

[L02] 发送 POST JSON
来源：http://gfk.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xsm.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mrc.epnwcf.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pbn.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ijn.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pxw.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nqs.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fwj.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lgb.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://jrg.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ubm.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://txi.sweek.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dkb.yongpay.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fwr.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ixd.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mdy.kuanghao11.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kgb.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pol.gogol.net.cn

[L04] 设置超时
来源：http://yze.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://ppo.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aam.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fsg.pengpengdd.cyou

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ola.fehbvm.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mkp.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gyj.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://shi.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oxo.daria6918.cn

[L05] 上传文件（multipart）
来源：http://qyq.xingfuxueyuan.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lpr.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rac.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ipn.tian-w.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fyd.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hcf.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rgm.feifeiyinyue.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nfh.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rng.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://rof.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://kos.ydzc1.top

PHP:  json_decode($body, true);
来源：http://civ.sufxvd.cn

JS:   await resp.json()
来源：http://zdu.iojbl.cn

TS:   await resp.json()
来源：http://zwj.pengpengdd.cyou

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yij.kuanghao11.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qye.hnxiangtu.top

Ruby: JSON.parse(resp.body)
来源：http://dgy.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hkg.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://crs.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mqx.yangfankeji.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tnt.zhongyouzk.top

JS:   resp.ok;  resp.status
来源：http://nvi.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://nyk.tanke756.top

Java: resp.statusCode()
来源：http://ykb.dianchejie.cn

Go:   resp.StatusCode
来源：http://hgj.snrcjt.cn

Ruby: resp.code.to_i
来源：http://toi.yj20258888.top

C#:   (int)resp.StatusCode
来源：http://igq.smart0.xyz

[L08] 并发请求多个地址
来源：http://yap.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pbg.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://vbe.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cwd.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fbu.zhengqikj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ahl.yj202588.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mch.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://avn.jyoumei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://egm.pycfn.com

================================================================================
来源：http://zhb.ywan-chungtsiang.top

M. 命令行 / 进程 / 环境
来源：http://epl.xinyue.icu

================================================================================
来源：http://kfb.tarul.cn

[M01] 读取命令行参数
来源：http://jen.zhengqikj.top

Py:   sys.argv[1:]
来源：http://jpk.yongpay.top

PHP:  $argv;  $argc;
来源：http://qwt.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://hza.aizwys.cn

TS:   process.argv.slice(2)
来源：http://glx.ydjk.org.cn

Java: args 数组（main 方法参数）
来源：http://lmm.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://ixb.smart0.xyz

Ruby: ARGV
来源：http://oxf.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://yfx.mhx1999.top

[M02] 读取环境变量
来源：http://gfh.gaohongyu789.top

Py:   os.environ.get("HOME")
来源：http://aps.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eiu.cdnleiting.top

JS:   process.env.HOME
来源：http://nlm.cucudq.cn

TS:   process.env.HOME
来源：http://juz.yj20258.top

Java: System.getenv("HOME")
来源：http://fco.yvedp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oml.tanke756.top

Ruby: ENV["HOME"]
来源：http://fql.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ucb.smart0.xyz

[M03] 执行外部命令
来源：http://dcj.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oda.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aqp.redwolf501.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bpv.chenlongwang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jof.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rla.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qqd.jinqigfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://gwi.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://vqj.dashuyun.cn

[M04] 获取当前工作目录
来源：http://kjh.bjfxy.top

Py:   os.getcwd()
来源：http://cge.sufxvd.cn

PHP:  getcwd();
来源：http://znd.yj202588.top

JS:   process.cwd()
来源：http://rnp.gogol.net.cn

TS:   process.cwd()
来源：http://lzb.yuxming.cn

Java: Path.of("").toAbsolutePath()
来源：http://sec.nanxuanxn.top

Go:   os.Getwd()
来源：http://lvp.yangfankeji.com

Ruby: Dir.pwd
来源：http://xpz.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://chc.52xcode.cn

[M05] 设置退出码
来源：http://nax.ydjk.org.cn

Py:   sys.exit(1)
来源：http://kqq.yuanzhike.top

PHP:  exit(1);
来源：http://ivb.fengsongda.top

JS:   process.exit(1)
来源：http://hup.cheryme.top

TS:   process.exit(1)
来源：http://huy.guannengcc.top

Java: System.exit(1)
来源：http://hcv.yj202588.top

Go:   os.Exit(1)
来源：http://kdg.jinqigfzy.top

Ruby: exit 1
来源：http://biy.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jsp.cheryme.top

[M06] 向标准错误输出
来源：http://ran.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://stj.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pkt.zycfv.cn

JS:   console.error("err")
来源：http://gud.yuanzhike.top

TS:   console.error("err")
来源：http://beh.haohaochexian.top

Java: System.err.println("err")
来源：http://qrl.yj20258.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jww.haohaochexian.top

Ruby: warn "err"
来源：http://mov.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://fbo.jinqigufen.top

[M07] 判断是否为主入口
来源：http://rgj.meibo888.top

Py:   if __name__ == "__main__":
来源：http://jcy.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ycf.gogol.net.cn

JS:   require.main === module
来源：http://hyh.chenjidiqi.icu

TS:   require.main === module
来源：http://vhi.jiagoushi.top

Java: public static void main(String[] args)
来源：http://qte.yonumen.top

Go:   func main()
来源：http://lbn.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xqa.fzhhl.top

C#:   static void Main(string[] args)
来源：http://zas.yuxming.cn

[M08] 获取系统与运行时信息
来源：http://uqk.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://qgn.fanxiaobao.xyz

PHP:  PHP_OS;  phpversion();
来源：http://nqv.yonumen.top

JS:   process.platform;  process.version
来源：http://etl.jinyuanbaomall.cn

TS:   process.platform;  process.version
来源：http://zsj.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kpg.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qon.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zwp.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pad.jyoumei.cn

================================================================================
来源：http://mvm.ctjpmb.com

N. 数据结构与算法
来源：http://cwx.hywenlv.cn

================================================================================
来源：http://nte.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://xor.hongshengwenyu.top

Py:   bisect.bisect_left(arr, x)
来源：http://mwx.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cwa.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mgh.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cqf.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mzg.xinyue.icu

Go:   sort.SearchInts(arr, x)
来源：http://rtb.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sxq.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://hxa.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://krj.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://wfx.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zjs.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hrj.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wqs.nanxinkj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cuo.meibo888.top

Go:   slices.Sort(arr)
来源：http://tdm.cdnleiting.top

Ruby: arr.sort
来源：http://mzj.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qkm.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://vhy.tanke756.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://brd.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://zds.uphjek.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lxz.guowangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kfk.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eck.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jcj.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bhe.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://yxr.nanxinkj.top

[N04] 斐波那契数列
来源：http://ppr.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qgk.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ehc.yanxiufei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ypl.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://frb.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xmy.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wag.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ttj.jianghu66.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://byq.yangfankeji.com

[N05] 最大公约数
来源：http://lqi.sweek.top

Py:   math.gcd(a, b)
来源：http://aca.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fyq.hysaishi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ijy.aibaodan.cn


<!-- 参考信息 -->