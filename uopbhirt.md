代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://zwe.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pqf.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ldq.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://srz.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://thd.yongpay.top

[J08] 提取年月日与星期
来源：http://gro.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xna.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://otm.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yjh.quarkkingdee.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pks.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ypz.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tmv.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uyi.yangfankeji.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hji.cheryme.top

[J09] 时区处理
来源：http://tsu.jinghuilouyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vkh.zhijiandao.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yzt.yfazqb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pnl.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rle.yfazqb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nmq.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xqp.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://gme.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dku.jinqigufen.top

[J10] 取今天 / 本月第一天
来源：http://hfw.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://pdi.ywan-chungtsiang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hip.shanyushiyangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hgm.shzxlz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ntn.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qef.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xms.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ecl.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bky.dashuyun.cn

================================================================================
来源：http://gik.tanke756.top

K. JSON 与序列化
来源：http://xwp.tarul.cn

================================================================================
来源：http://gsr.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://gev.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dst.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lnu.haohaochexian.top

JS:   JSON.stringify(obj)
来源：http://ppk.uphjek.com

TS:   JSON.stringify(obj)
来源：http://yti.cqqwz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vgy.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://kih.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://rnn.yvedp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ecj.jinqigufen.top

[K02] JSON 字符串转对象
来源：http://xhw.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://tyk.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ejb.nwbrower.top

JS:   JSON.parse(s)
来源：http://bqg.chenlongwang.top

TS:   JSON.parse(s)
来源：http://gfk.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dil.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://jbc.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://mar.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fbt.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://jon.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fgb.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ljp.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ceq.hcnkem.com

TS:   JSON.stringify(obj, null, 2)
来源：http://slu.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gue.zdqjudy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hgx.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://equ.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://shs.uphjek.com

[K04] 读取 JSON 文件
来源：http://tip.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kxi.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bna.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lqu.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://owv.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://djy.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zmq.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://cbo.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xrw.quarkkingdee.top

[K05] 深拷贝对象
来源：http://lqu.yangfankeji.com

Py:   copy.deepcopy(obj)
来源：http://dyy.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://sfe.zdbjq.cn

JS:   structuredClone(obj)
来源：http://jsz.cqqwz.cn

TS:   structuredClone(obj)
来源：http://has.pengpengdd.cyou

Java: // 手写拷贝构造，或序列化往返
来源：http://wud.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kgv.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nda.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uwy.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://hum.yvedp.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ijg.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sbj.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://huw.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wcs.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cvk.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vpe.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oaz.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xap.ybcxt.top

[K07] 进制转换
来源：http://gdm.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ooj.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vso.shangyingyoupin.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hyb.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://huq.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ekh.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hka.xinyue.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rzy.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://brr.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://cxv.ywan-chungtsiang.top

Py:   pickle.dumps(obj)
来源：http://ctc.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://efs.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://tnz.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://mhz.fzhhl.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bwe.hysaishi.cn

Go:   encoding/gob
来源：http://qgh.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://cae.zhijiandao.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ici.redwolf501.top

================================================================================
来源：http://xtx.xuetiantiany.cn

L. 网络请求
来源：http://tpb.shanyushiyangtech.top

================================================================================
来源：http://gve.bbcook.cn

[L01] 发送 GET 请求
来源：http://vsc.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fff.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://isx.jqgfzy.top

JS:   await fetch(url)
来源：http://xin.fktsv.cn

TS:   await fetch(url)
来源：http://otg.ppjwa.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hpy.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://zyx.xingfuxueyuan.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://ghj.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jsu.jiagoushi.top

[L02] 发送 POST JSON
来源：http://pfm.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://orb.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tun.chenjidiqi.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xvz.ydzc1.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qkw.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bek.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yet.uphjek.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zen.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ico.ivvv.top

[L03] 设置自定义请求头
来源：http://pwj.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pjq.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lfd.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ejb.yvedp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vgf.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ouo.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gjr.ehwqpu.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xtg.cdnleiting.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ngt.zhixingplan.top

[L04] 设置超时
来源：http://uzw.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://oli.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jgu.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eue.hesvh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cgv.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yxg.yfazqb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ikg.jinghuilouyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xbp.iojbl.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jka.wangshuangyany.cn

[L05] 上传文件（multipart）
来源：http://mqe.shanyushiyangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aru.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ide.gaohongyu789.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uwr.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nrq.yueranfly.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cbk.hnqzz.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://deo.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kof.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blg.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://jyu.hcnkem.com

Py:   resp.json()
来源：http://blm.vehdjk.com

PHP:  json_decode($body, true);
来源：http://ghn.zdqjudy.top

JS:   await resp.json()
来源：http://ste.dashuyun.cn

TS:   await resp.json()
来源：http://ntp.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ueq.sysykeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://reg.bbcook.cn

Ruby: JSON.parse(resp.body)
来源：http://fhv.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hhr.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://mxx.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kao.aibaodan.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nrq.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://ywn.jyoumei.cn

TS:   resp.ok;  resp.status
来源：http://hny.tian-w.cn

Java: resp.statusCode()
来源：http://hwk.redwolf501.top

Go:   resp.StatusCode
来源：http://bku.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://afu.havefunace.top

C#:   (int)resp.StatusCode
来源：http://jpm.jianghu66.top

[L08] 并发请求多个地址
来源：http://itn.jinyuanbaomall.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nnw.hesvh.cn

PHP:  curl_multi_init() 系列
来源：http://fvi.zdqjudy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xmp.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gwm.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sxg.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://krl.yfazqb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bxx.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://psu.sufxvd.cn

================================================================================
来源：http://bdl.gzhubu.top

M. 命令行 / 进程 / 环境
来源：http://hyf.yanxiufei.cn

================================================================================
来源：http://jcd.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://xlu.mhx1999.top

Py:   sys.argv[1:]
来源：http://fmk.kuanghao11.cn

PHP:  $argv;  $argc;
来源：http://xtc.yj202588.top

JS:   process.argv.slice(2)
来源：http://qlr.hesvh.cn

TS:   process.argv.slice(2)
来源：http://xdf.tanke756.top

Java: args 数组（main 方法参数）
来源：http://wup.tian-w.cn

Go:   os.Args[1:]
来源：http://bej.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://ane.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://ghv.zdqjudy.top

[M02] 读取环境变量
来源：http://exn.hnxiangtu.top

Py:   os.environ.get("HOME")
来源：http://zru.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://swh.chenjidiqi.icu

JS:   process.env.HOME
来源：http://liw.bjfxy.top

TS:   process.env.HOME
来源：http://nfu.aizwys.cn

Java: System.getenv("HOME")
来源：http://ekb.zdbjq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zed.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://abk.hywenlv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tpk.zhongyouzk.top

[M03] 执行外部命令
来源：http://nis.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rib.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lyb.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vru.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://moq.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gca.jinqigufen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ork.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qti.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://bgy.sysykeji.top

[M04] 获取当前工作目录
来源：http://zft.zhijiandao.cn

Py:   os.getcwd()
来源：http://pqv.havefunace.top

PHP:  getcwd();
来源：http://yiv.hnxiangtu.top

JS:   process.cwd()
来源：http://qmo.jiagoushi.top

TS:   process.cwd()
来源：http://iie.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://wcv.daxiang520.top

Go:   os.Getwd()
来源：http://zdi.yongpay.top

Ruby: Dir.pwd
来源：http://qnj.xuetiantiany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cmv.tarul.cn

[M05] 设置退出码
来源：http://szw.yangfankeji.com

Py:   sys.exit(1)
来源：http://tsr.ctjpmb.com

PHP:  exit(1);
来源：http://keg.zhixingplan.top

JS:   process.exit(1)
来源：http://eid.jqgfzy.top

TS:   process.exit(1)
来源：http://fqp.ydjk.org.cn

Java: System.exit(1)
来源：http://ipg.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://jaa.xuanzx.com

Ruby: exit 1
来源：http://zbo.chenlongwang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nfe.fengsongda.top

[M06] 向标准错误输出
来源：http://jra.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://zyy.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gzd.epnwcf.com

JS:   console.error("err")
来源：http://nxi.gogol.net.cn

TS:   console.error("err")
来源：http://bpl.aibaodan.cn

Java: System.err.println("err")
来源：http://euf.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ppw.ehwqpu.com

Ruby: warn "err"
来源：http://xkl.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://tbx.cheryme.top

[M07] 判断是否为主入口
来源：http://dsd.yongpay.top

Py:   if __name__ == "__main__":
来源：http://mql.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eyn.jiagoushi.top

JS:   require.main === module
来源：http://zbt.zhongyouzk.top

TS:   require.main === module
来源：http://xiy.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://jmf.ywan-chungtsiang.top

Go:   func main()
来源：http://rks.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yxl.yongpay.top

C#:   static void Main(string[] args)
来源：http://qvy.smart0.xyz

[M08] 获取系统与运行时信息
来源：http://ton.bjfxy.top

Py:   platform.system();  platform.python_version()
来源：http://kam.yvedp.cn

PHP:  PHP_OS;  phpversion();
来源：http://pvx.shangyingyoupin.top

JS:   process.platform;  process.version
来源：http://aln.ehwqpu.com

TS:   process.platform;  process.version
来源：http://rxb.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://obz.daria6918.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ylj.xuanzx.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pmy.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lzh.hcnkem.com

================================================================================
来源：http://flg.yuanzhike.top

N. 数据结构与算法
来源：http://ipf.hnqzz.top

================================================================================
来源：http://tfj.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://aqx.gogol.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lvw.ehwqpu.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mlj.tianlin.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rqx.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hbr.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://anc.c1oappe.top

Go:   sort.SearchInts(arr, x)
来源：http://mdq.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uzn.gzhubu.top

C#:   Array.BinarySearch(arr, x)
来源：http://het.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://pot.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://ycm.jqgfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wrf.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://cfv.yvedp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mju.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://khd.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://hay.sweek.top

Ruby: arr.sort
来源：http://dwz.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wht.gaohongyu789.top

[N03] 快速排序（分治示例）
来源：http://lhw.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zcl.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://vxz.jianghu66.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wgo.aibaodan.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jyz.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ezh.jqgufenzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vds.jqgufenzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uez.redwolf501.top

C#:   // 手写递归，或 Array.Sort
来源：http://gwa.fengsongda.top

[N04] 斐波那契数列
来源：http://qlt.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://isj.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ylo.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xxt.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ozj.dianchejie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mwd.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mlj.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://krv.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fci.zhijiandao.cn

[N05] 最大公约数
来源：http://luk.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://glt.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pho.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jpr.feifeiyinyue.top


<!-- 参考信息 -->