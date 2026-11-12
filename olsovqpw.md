代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://vjj.hnqzz.top

[J08] 提取年月日与星期
来源：http://yrt.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dyz.yj20258888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xvp.epnwcf.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kfa.cdnleiting.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://acs.fzhhl.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ujz.dashuyun.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://poq.shanyushiyangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eoh.jqgufenzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gbu.shzxlz.cn

[J09] 时区处理
来源：http://opa.jqgufenzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ugw.xziqi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sqq.ppjwa.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mri.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vtw.jinghuilouyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bif.tianlin.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://acp.dianchejie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gta.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rmy.haohaochexian.top

[J10] 取今天 / 本月第一天
来源：http://vud.zhijiandao.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yne.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wlt.bbcook.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ltd.9152youxi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rnh.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://khq.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ndf.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wju.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nfe.chenzaomai.com

================================================================================
来源：http://ahr.sweek.top

K. JSON 与序列化
来源：http://pbl.redwolf501.top

================================================================================
来源：http://mjs.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://cjy.cqqwz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://low.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dgr.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://aep.yonumen.top

TS:   JSON.stringify(obj)
来源：http://hqb.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sfr.bjfxy.top

Go:   json.Marshal(obj)
来源：http://yqh.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://mrp.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://unp.mhx1999.top

[K02] JSON 字符串转对象
来源：http://jdt.chenlongwang.top

Py:   json.loads(s)
来源：http://jqy.gotoacloud.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nqg.epnwcf.com

JS:   JSON.parse(s)
来源：http://iae.zhaomingkeji.xyz

TS:   JSON.parse(s)
来源：http://dbm.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://prx.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://efr.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://tal.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rnr.hysaishi.cn

[K03] JSON 美化输出（带缩进）
来源：http://omv.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://txm.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hgy.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ohv.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ywr.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gvl.hammf.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fef.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://lef.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bgz.dianchejie.cn

[K04] 读取 JSON 文件
来源：http://pyb.ivvv.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rpm.zhiwuduotai.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nuw.bbcook.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yqg.yvedp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kjq.zdqjudy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zil.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ntn.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://qnl.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kun.snrcjt.cn

[K05] 深拷贝对象
来源：http://ixl.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://okf.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://zbx.cdnleiting.top

JS:   structuredClone(obj)
来源：http://tnj.feifeiyinyue.top

TS:   structuredClone(obj)
来源：http://qfw.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://aqf.bbcook.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://usf.hesvh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ugz.wangshuangyany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fxw.hnqzz.top

[K06] 解析 URL 查询串
来源：http://dmp.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://win.smart0.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hvn.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bgc.sysykeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bcm.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tox.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mpy.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yke.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zux.9152youxi.cn

[K07] 进制转换
来源：http://bcb.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pwp.316326.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yrz.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pxx.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pfs.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pyq.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tao.zhongyouzk.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rjl.chenzaomai.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://raw.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://bae.pycfn.com

Py:   pickle.dumps(obj)
来源：http://llk.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://prt.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://whb.hnxiangtu.top

TS:   v8.serialize(obj)        // Node
来源：http://xai.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://epe.hnqzz.top

Go:   encoding/gob
来源：http://zmf.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://fps.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eku.yj202588.top

================================================================================
来源：http://exm.chenzaomai.com

L. 网络请求
来源：http://jdn.haohaochexian.top

================================================================================
来源：http://pws.wangdashe.top

[L01] 发送 GET 请求
来源：http://vlj.yangfankeji.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fep.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kda.xinyue.icu

JS:   await fetch(url)
来源：http://fur.hesvh.cn

TS:   await fetch(url)
来源：http://rtk.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gpt.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://qsa.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rss.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rau.gotoacloud.top

[L02] 发送 POST JSON
来源：http://cja.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ilp.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fcw.yvedp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zcj.shanyushiyangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zpn.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rqc.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://duj.sxryk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aoo.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dmt.ehwqpu.com

[L03] 设置自定义请求头
来源：http://afc.fzhhl.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://edz.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jor.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kdr.zhaomingkeji.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ute.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tdv.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bns.hongshengwenyu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oty.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dal.gzhubu.top

[L04] 设置超时
来源：http://dli.kuanghao11.cn

Py:   requests.get(url, timeout=5)
来源：http://pgr.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ujw.jinqigfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mbs.xinyue.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://byf.bbcook.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lsg.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kxp.chenlongwang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ufr.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zhl.zycfv.cn

[L05] 上传文件（multipart）
来源：http://gmw.uphjek.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fml.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hia.cheryme.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xfo.pycfn.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ufq.ivvv.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bxz.hnqzz.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hfy.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tgd.ydjk.org.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://niw.xingfuxueyuan.xyz

[L06] 解析响应为 JSON
来源：http://yfh.hysaishi.cn

Py:   resp.json()
来源：http://dxe.hammf.cn

PHP:  json_decode($body, true);
来源：http://nwx.zhijiandao.cn

JS:   await resp.json()
来源：http://fnb.sysykeji.top

TS:   await resp.json()
来源：http://dvf.meibo888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gbk.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pxo.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://evy.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://utq.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://lsg.havefunace.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gnj.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yfb.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://opa.xuetiantiany.cn

TS:   resp.ok;  resp.status
来源：http://jxn.jinqigfzy.top

Java: resp.statusCode()
来源：http://upc.zhijiandao.cn

Go:   resp.StatusCode
来源：http://wzg.chenjidiqi.icu

Ruby: resp.code.to_i
来源：http://srm.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://rka.ybcxt.top

[L08] 并发请求多个地址
来源：http://gmh.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ijf.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://bzh.shuidangran.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cap.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jmk.shangyingyoupin.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://txl.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fee.sweek.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kdg.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iqd.ivvv.top

================================================================================
来源：http://xsg.zdqjudy.top

M. 命令行 / 进程 / 环境
来源：http://cfs.hongshengwenyu.top

================================================================================
来源：http://nco.tianlin.xyz

[M01] 读取命令行参数
来源：http://aoj.cqqwz.cn

Py:   sys.argv[1:]
来源：http://nfd.pycfn.com

PHP:  $argv;  $argc;
来源：http://lkm.shuidangran.top

JS:   process.argv.slice(2)
来源：http://khq.zhengqikj.top

TS:   process.argv.slice(2)
来源：http://bat.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://pbt.pycfn.com

Go:   os.Args[1:]
来源：http://fwk.dashuyun.cn

Ruby: ARGV
来源：http://xxg.guowangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://sxm.fehbvm.com

[M02] 读取环境变量
来源：http://eis.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://qww.shangyingyoupin.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://clu.birdmap.top

JS:   process.env.HOME
来源：http://gcm.aizwys.cn

TS:   process.env.HOME
来源：http://qua.hnxiangtu.top

Java: System.getenv("HOME")
来源：http://vbr.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yis.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://qlt.jiagoushi.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kej.fengsongda.top

[M03] 执行外部命令
来源：http://xea.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lkz.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hyh.shanyushiyangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tgr.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bfl.hcnkem.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yqb.dashuyun.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uzg.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://zcc.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://yid.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://cie.hcnkem.com

Py:   os.getcwd()
来源：http://gtz.havefunace.top

PHP:  getcwd();
来源：http://amq.dianchejie.cn

JS:   process.cwd()
来源：http://tcn.meibo888.top

TS:   process.cwd()
来源：http://oll.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://fca.yfazqb.com

Go:   os.Getwd()
来源：http://dhq.shuidangran.top

Ruby: Dir.pwd
来源：http://fsf.smart0.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://tpq.uphjek.com

[M05] 设置退出码
来源：http://nut.yvedp.cn

Py:   sys.exit(1)
来源：http://zev.0kj1m.cn

PHP:  exit(1);
来源：http://oyk.fzhhl.top

JS:   process.exit(1)
来源：http://tby.aizwys.cn

TS:   process.exit(1)
来源：http://dcj.zdbjq.cn

Java: System.exit(1)
来源：http://epm.yuxming.cn

Go:   os.Exit(1)
来源：http://cpm.gaohongyu789.top

Ruby: exit 1
来源：http://mty.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ely.ywan-chungtsiang.top

[M06] 向标准错误输出
来源：http://vup.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://frl.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ksz.uphjek.com

JS:   console.error("err")
来源：http://zgw.52xcode.cn

TS:   console.error("err")
来源：http://npf.jiagoushi.top

Java: System.err.println("err")
来源：http://lje.zhaomingkeji.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lvp.cashguo.top

Ruby: warn "err"
来源：http://izr.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://zzh.hnxiangtu.top

[M07] 判断是否为主入口
来源：http://nmr.yj20258.top

Py:   if __name__ == "__main__":
来源：http://fki.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wyw.gaohongyu789.top

JS:   require.main === module
来源：http://wpp.ydjk.org.cn

TS:   require.main === module
来源：http://wbr.tianlin.xyz

Java: public static void main(String[] args)
来源：http://wrv.zdqjudy.top

Go:   func main()
来源：http://glw.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yvg.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://hlg.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://nka.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://xuq.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://jdv.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://nyr.chenjidiqi.icu

TS:   process.platform;  process.version
来源：http://zsu.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mdl.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pix.xuanzx.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kgm.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ofl.jlsjyb.cn

================================================================================
来源：http://ikb.shzxlz.cn

N. 数据结构与算法
来源：http://mft.hcnkem.com

================================================================================
来源：http://usb.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://ovl.ivvv.top

Py:   bisect.bisect_left(arr, x)
来源：http://kua.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://srr.sweek.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lau.guowangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yqk.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mry.xingfuxueyuan.xyz

Go:   sort.SearchInts(arr, x)
来源：http://bsr.yj20258.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ual.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://rte.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://mqu.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://jbc.shuidangran.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sgn.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xau.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jkb.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zng.zhijiandao.cn

Go:   slices.Sort(arr)
来源：http://mcy.yj202588.top

Ruby: arr.sort
来源：http://tyg.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mpt.yanxiufei.cn

[N03] 快速排序（分治示例）
来源：http://kps.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yoo.yueranfly.top

PHP:  // 递归实现，或用 usort
来源：http://xcl.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tzz.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://avy.shangyingyoupin.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dif.zycfv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hlb.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dic.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://uwk.zhiwuduotai.top

[N04] 斐波那契数列
来源：http://bvr.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dvw.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rkd.shuidangran.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://okg.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qai.zhiwuduotai.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oym.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mdz.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tep.daxiang520.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zkx.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://sqz.zhongyouzk.top

Py:   math.gcd(a, b)
来源：http://zdb.tarul.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oki.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eqq.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qkn.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wqd.bbcook.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wev.redwolf501.top

Ruby: a.gcd(b)
来源：http://dvr.feifeiyinyue.top


<!-- 参考信息 -->