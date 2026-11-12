代发 wailian999

[J07] 比较两个日期
来源：http://dqk.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://qul.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xtz.ybcxt.top

JS:   d1.getTime() < d2.getTime()
来源：http://jde.jyoumei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ekt.nanxuanxn.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vbm.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iee.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wnp.fzhhl.top

C#:   d1 < d2;  d1 == d2
来源：http://afg.yuanzhike.top

[J08] 提取年月日与星期
来源：http://wdz.hesvh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bhu.c1oappe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rdx.quarkkingdee.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lhx.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://awe.feifeiyinyue.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ztq.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bnh.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tyg.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://azg.zhiwuduotai.top

[J09] 时区处理
来源：http://jtp.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://okt.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sxu.meibo888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hgx.c1oappe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cgo.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ebw.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tnh.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fyo.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mgo.shanyushiyangkeji.top

[J10] 取今天 / 本月第一天
来源：http://huo.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://xxh.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://abk.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tom.jinyuanbaomall.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://spo.vehdjk.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zqk.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ete.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kmr.ehwqpu.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mks.c1oappe.top

================================================================================
来源：http://slp.zhijiandao.cn

K. JSON 与序列化
来源：http://zwu.vehdjk.com

================================================================================
来源：http://gdb.hysaishi.cn

[K01] 对象转 JSON 字符串
来源：http://wck.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ftz.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wkn.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://ldo.yj202588.top

TS:   JSON.stringify(obj)
来源：http://ahv.zhengqikj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jdv.haohaochexian.top

Go:   json.Marshal(obj)
来源：http://cap.andypj.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://nga.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://txe.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://ezt.hcnkem.com

Py:   json.loads(s)
来源：http://ppc.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://upk.tianlin.xyz

JS:   JSON.parse(s)
来源：http://rfa.yongpay.top

TS:   JSON.parse(s)
来源：http://hyf.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kst.zdbjq.cn

Go:   json.Unmarshal(data, &v)
来源：http://ivg.cheryme.top

Ruby: JSON.parse(s)
来源：http://inn.uphjek.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mfa.hongshengwenyu.top

[K03] JSON 美化输出（带缩进）
来源：http://grx.yueranfly.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wfa.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mne.52xcode.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zxp.aizwys.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://qpt.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yrs.ybcxt.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pjm.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://jnm.gotoacloud.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://abd.guowangkeji.top

[K04] 读取 JSON 文件
来源：http://izt.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pyi.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lmn.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xrn.0kj1m.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fum.gaohongyu789.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://djt.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hvv.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bqf.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zgx.zhoulong.xyz

[K05] 深拷贝对象
来源：http://vkl.zdqjudy.top

Py:   copy.deepcopy(obj)
来源：http://bze.jinghuilouyu.cn

PHP:  unserialize(serialize($obj));
来源：http://gnx.yfazqb.com

JS:   structuredClone(obj)
来源：http://icq.xylfe.cn

TS:   structuredClone(obj)
来源：http://zuv.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ryn.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bub.uphjek.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kfa.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://akp.yfazqb.com

[K06] 解析 URL 查询串
来源：http://roz.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kxj.epnwcf.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gwl.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hos.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ljj.tian-w.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zbq.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rue.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ppf.hammf.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yci.xylfe.cn

[K07] 进制转换
来源：http://whx.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wye.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ltc.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bcx.nwbrower.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lci.0kj1m.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zru.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tfw.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ovr.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yvj.sufxvd.cn

[K08] 二进制序列化（非 JSON）
来源：http://gxu.shuidangran.top

Py:   pickle.dumps(obj)
来源：http://cpz.gogol.net.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dnb.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://iux.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://noe.iojbl.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vck.dianchejie.cn

Go:   encoding/gob
来源：http://kit.xylfe.cn

Ruby: Marshal.dump(obj)
来源：http://aop.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://avk.andypj.xyz

================================================================================
来源：http://nud.cucudq.cn

L. 网络请求
来源：http://lop.zhengqikj.top

================================================================================
来源：http://nox.yongpay.top

[L01] 发送 GET 请求
来源：http://ffp.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://slt.zhongyouzk.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nqp.zhoulong.xyz

JS:   await fetch(url)
来源：http://ohm.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://atq.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pqs.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://fpg.xuanzx.com

Ruby: Net::HTTP.get(URI(url))
来源：http://snq.daria6918.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gcc.svipenyu.cn

[L02] 发送 POST JSON
来源：http://eml.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://eui.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fkn.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ksw.gogol.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bkt.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vvd.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hdq.jianghu66.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://edm.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://grr.gogol.net.cn

[L03] 设置自定义请求头
来源：http://yqu.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pjp.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lfu.shanyushiyangtech.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fiv.shanyushiyangtech.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hzg.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://via.vehdjk.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://skn.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://znm.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kup.52xcode.cn

[L04] 设置超时
来源：http://qmh.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://cnu.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://esf.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dwt.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hrd.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ees.yangfankeji.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tci.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://whl.52xcode.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jkq.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://ura.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rww.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sun.gogol.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gyo.snrcjt.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://egf.9152youxi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ldl.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fku.cheryme.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://juq.epnwcf.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://khx.316326.xyz

[L06] 解析响应为 JSON
来源：http://ueh.epnwcf.com

Py:   resp.json()
来源：http://osu.aizwys.cn

PHP:  json_decode($body, true);
来源：http://szw.gogol.net.cn

JS:   await resp.json()
来源：http://pzu.hcnkem.com

TS:   await resp.json()
来源：http://ltr.guowangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rdk.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wzo.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://jkl.zycfv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ifw.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://ftp.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tvg.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ufx.chenlongwang.top

JS:   resp.ok;  resp.status
来源：http://kiw.hcnkem.com

TS:   resp.ok;  resp.status
来源：http://twr.feifeiyinyue.top

Java: resp.statusCode()
来源：http://szb.guannengcc.top

Go:   resp.StatusCode
来源：http://fif.zdqjudy.top

Ruby: resp.code.to_i
来源：http://gqg.feifeiyinyue.top

C#:   (int)resp.StatusCode
来源：http://bvm.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://zrk.hongshengwenyu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ymr.aibaodan.cn

PHP:  curl_multi_init() 系列
来源：http://voi.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fia.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cui.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dcb.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kje.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uhz.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://syf.fzhhl.top

================================================================================
来源：http://zzf.yj20258888.top

M. 命令行 / 进程 / 环境
来源：http://acs.ivvv.top

================================================================================
来源：http://ljg.yj202588.top

[M01] 读取命令行参数
来源：http://rmh.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://epc.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://avw.yvedp.cn

JS:   process.argv.slice(2)
来源：http://qwe.c1oappe.top

TS:   process.argv.slice(2)
来源：http://cjp.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://lhs.jinqigufen.top

Go:   os.Args[1:]
来源：http://iek.bbcook.cn

Ruby: ARGV
来源：http://cit.sjlbkw.cn

C#:   args 数组（Main 方法参数）
来源：http://sox.ybcxt.top

[M02] 读取环境变量
来源：http://lud.gaohongyu789.top

Py:   os.environ.get("HOME")
来源：http://qps.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cyo.guannengcc.top

JS:   process.env.HOME
来源：http://ede.dianchejie.cn

TS:   process.env.HOME
来源：http://cuz.yvedp.cn

Java: System.getenv("HOME")
来源：http://rkh.daxiang520.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ebw.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://qdp.xuetiantiany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jjq.wangshuangyany.cn

[M03] 执行外部命令
来源：http://ima.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://isa.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ubq.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://snf.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://hph.bbcook.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iey.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pty.zhijiandao.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tng.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://tpb.sysykeji.top

[M04] 获取当前工作目录
来源：http://jdc.shanyushiyangtech.top

Py:   os.getcwd()
来源：http://yut.svipenyu.cn

PHP:  getcwd();
来源：http://ugu.yongpay.top

JS:   process.cwd()
来源：http://kvt.sysykeji.top

TS:   process.cwd()
来源：http://lpq.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://jhm.xuanzx.com

Go:   os.Getwd()
来源：http://vyd.gzhubu.top

Ruby: Dir.pwd
来源：http://zww.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iwf.aizwys.cn

[M05] 设置退出码
来源：http://xpi.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://fox.chenjidiqi.icu

PHP:  exit(1);
来源：http://szg.zhoulong.xyz

JS:   process.exit(1)
来源：http://ich.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://rad.hesvh.cn

Java: System.exit(1)
来源：http://fzk.9152youxi.cn

Go:   os.Exit(1)
来源：http://spm.daxiang520.top

Ruby: exit 1
来源：http://jqo.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bit.gotoacloud.top

[M06] 向标准错误输出
来源：http://flt.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://bmh.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xqv.zdbjq.cn

JS:   console.error("err")
来源：http://drw.gotoacloud.top

TS:   console.error("err")
来源：http://spe.9152youxi.cn

Java: System.err.println("err")
来源：http://bqm.guannengcc.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kuu.9152youxi.cn

Ruby: warn "err"
来源：http://cxk.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://wov.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://byq.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://lmw.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kfh.yvedp.cn

JS:   require.main === module
来源：http://ujx.andypj.xyz

TS:   require.main === module
来源：http://mav.shangyingyoupin.top

Java: public static void main(String[] args)
来源：http://bpf.yj20258.top

Go:   func main()
来源：http://njd.jlsjyb.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ggn.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://ahl.yuanzhike.top

[M08] 获取系统与运行时信息
来源：http://yws.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://hgu.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://xef.chenzaomai.com

JS:   process.platform;  process.version
来源：http://rzt.fzhhl.top

TS:   process.platform;  process.version
来源：http://jzv.gotoacloud.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ajn.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tyc.fengsongda.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bac.hnqzz.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ans.xylfe.cn

================================================================================
来源：http://ftm.cheryme.top

N. 数据结构与算法
来源：http://yqd.ydzc1.top

================================================================================
来源：http://kmb.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://byz.zhixingplan.top

Py:   bisect.bisect_left(arr, x)
来源：http://tem.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kks.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gti.yanxiufei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qqx.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tyy.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://xcu.yangfankeji.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ukz.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://duk.xinyue.icu

[N02] 排序（工程实践用内置实现）
来源：http://eny.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://anb.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cln.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fkz.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xyo.shangyingyoupin.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://apj.xziqi.cn

Go:   slices.Sort(arr)
来源：http://dhb.c1oappe.top

Ruby: arr.sort
来源：http://giz.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://igu.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://lau.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ywj.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://uwc.gogol.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rrp.fanxiaobao.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fbq.dashuyun.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://unt.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://awv.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uni.xingfuxueyuan.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://evx.fzhhl.top

[N04] 斐波那契数列
来源：http://bdk.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mnh.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://adx.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://log.redwolf501.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dkf.haohaochexian.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://czl.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zey.shzxlz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iii.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qjg.jqgfzy.top


<!-- 参考信息 -->