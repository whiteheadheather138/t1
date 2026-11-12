代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wdl.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://imw.ehwqpu.com

[J09] 时区处理
来源：http://cjb.gotoacloud.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hgy.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bmg.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fvf.fanxiaobao.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nkz.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xfj.ppjwa.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ryq.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vjh.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fjz.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://dor.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ach.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ppu.aibaodan.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ukn.hesvh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xiz.fanxiaobao.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qpv.52xcode.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ppr.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mqx.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nfg.yanxiufei.cn

================================================================================
来源：http://saa.iojbl.cn

K. JSON 与序列化
来源：http://bcx.yongpay.top

================================================================================
来源：http://yme.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://srf.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bzr.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fma.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://xlb.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://wbc.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://twe.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://ivk.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kjz.yvedp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ant.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://dvh.nanxinkj.top

Py:   json.loads(s)
来源：http://srb.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pkc.svipenyu.cn

JS:   JSON.parse(s)
来源：http://zlz.cdnleiting.top

TS:   JSON.parse(s)
来源：http://aef.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jwl.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://wsv.xuanzx.com

Ruby: JSON.parse(s)
来源：http://bog.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fkj.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://ycc.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ktv.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gnn.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://ptb.sweek.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xdt.52xcode.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://abt.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://amb.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://dqs.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tik.52xcode.cn

[K04] 读取 JSON 文件
来源：http://rnv.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://chs.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rmz.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wjy.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rif.yanxiufei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mij.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kto.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://byt.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qif.ehwqpu.com

[K05] 深拷贝对象
来源：http://aen.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://lvy.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://yja.cucudq.cn

JS:   structuredClone(obj)
来源：http://pgq.zhengqikj.top

TS:   structuredClone(obj)
来源：http://soj.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rgg.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ldk.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://byx.yj20258.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lhw.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://cox.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://drs.birdmap.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://clq.fanxiaobao.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://krd.yj20258.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vak.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dqs.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xyp.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fxl.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tsx.shanyushiyangkeji.top

[K07] 进制转换
来源：http://pct.quarkkingdee.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://egc.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fbg.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tfj.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lnm.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://inu.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ojw.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tyg.xinyue.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ddd.sysykeji.top

[K08] 二进制序列化（非 JSON）
来源：http://zht.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://ehy.fengsongda.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iev.hesvh.cn

JS:   v8.serialize(obj)        // Node
来源：http://wmi.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://ebn.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kxz.jiagoushi.top

Go:   encoding/gob
来源：http://pdp.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://hlf.tianlin.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jzx.zhaomingkeji.xyz

================================================================================
来源：http://crf.havefunace.top

L. 网络请求
来源：http://cpt.gzhubu.top

================================================================================
来源：http://nod.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://jvh.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tap.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gmp.vqdsnc.cn

JS:   await fetch(url)
来源：http://hle.yj20258888.top

TS:   await fetch(url)
来源：http://dxf.birdmap.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zsj.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://iut.bjfxy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lqa.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://anw.jqgfzy.top

[L02] 发送 POST JSON
来源：http://npl.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ity.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uqx.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yft.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tzm.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jat.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uqu.uphjek.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bna.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fxf.jqgufenzy.top

[L03] 设置自定义请求头
来源：http://czt.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mkt.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bug.uphjek.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://laz.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://owh.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ojk.shzxlz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jsy.haohaochexian.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cci.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kkc.zhoulong.xyz

[L04] 设置超时
来源：http://ctz.chenlongwang.top

Py:   requests.get(url, timeout=5)
来源：http://hmu.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pwx.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nvg.jyoumei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mdh.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cyp.havefunace.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://scm.9152youxi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://olq.c1oappe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jwm.birdmap.top

[L05] 上传文件（multipart）
来源：http://xnl.jinqigfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wyz.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tdz.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mvh.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xzb.jianghu66.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ema.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qol.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mct.tanke756.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yfi.nanxuanxn.top

[L06] 解析响应为 JSON
来源：http://kdv.nwbrower.top

Py:   resp.json()
来源：http://ppj.yanxiufei.cn

PHP:  json_decode($body, true);
来源：http://xrb.xziqi.cn

JS:   await resp.json()
来源：http://def.jinqigufen.top

TS:   await resp.json()
来源：http://jir.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oyd.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lcd.9152youxi.cn

Ruby: JSON.parse(resp.body)
来源：http://cdr.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ylc.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://wir.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qxe.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://emz.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://aef.pycfn.com

TS:   resp.ok;  resp.status
来源：http://bbt.havefunace.top

Java: resp.statusCode()
来源：http://syr.fehbvm.com

Go:   resp.StatusCode
来源：http://eyx.daria6918.cn

Ruby: resp.code.to_i
来源：http://fiv.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://xbz.fzhhl.top

[L08] 并发请求多个地址
来源：http://lsl.yfazqb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pxx.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://vof.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wiq.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://njp.fengsongda.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nnk.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hmw.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://awe.vqdsnc.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vmm.pengpengdd.cyou

================================================================================
来源：http://wzm.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://oal.havefunace.top

================================================================================
来源：http://kwg.jianghu66.top

[M01] 读取命令行参数
来源：http://kou.ivvv.top

Py:   sys.argv[1:]
来源：http://vky.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://dye.jianghu66.top

JS:   process.argv.slice(2)
来源：http://grn.c1oappe.top

TS:   process.argv.slice(2)
来源：http://ckv.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://fgn.aizwys.cn

Go:   os.Args[1:]
来源：http://jlu.sufxvd.cn

Ruby: ARGV
来源：http://fkz.dianchejie.cn

C#:   args 数组（Main 方法参数）
来源：http://sdb.xuetiantiany.cn

[M02] 读取环境变量
来源：http://uxu.aibaodan.cn

Py:   os.environ.get("HOME")
来源：http://vxo.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gvo.fktsv.cn

JS:   process.env.HOME
来源：http://uyx.cheryme.top

TS:   process.env.HOME
来源：http://mwr.snrcjt.cn

Java: System.getenv("HOME")
来源：http://ecp.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oec.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://nyh.hesvh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yyf.ydzc1.top

[M03] 执行外部命令
来源：http://fhu.birdmap.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vqz.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ckh.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://uld.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hur.pycfn.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qed.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uqk.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ruo.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://tng.yfazqb.com

[M04] 获取当前工作目录
来源：http://yvb.fehbvm.com

Py:   os.getcwd()
来源：http://lfe.jqgfzy.top

PHP:  getcwd();
来源：http://lqs.yanxiufei.cn

JS:   process.cwd()
来源：http://zqb.sufxvd.cn

TS:   process.cwd()
来源：http://khr.hammf.cn

Java: Path.of("").toAbsolutePath()
来源：http://pug.aibaodan.cn

Go:   os.Getwd()
来源：http://fgu.shzxlz.cn

Ruby: Dir.pwd
来源：http://qkb.sysykeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://kds.jinqigufen.top

[M05] 设置退出码
来源：http://kze.cashguo.top

Py:   sys.exit(1)
来源：http://yaa.redwolf501.top

PHP:  exit(1);
来源：http://aou.feifeiyinyue.top

JS:   process.exit(1)
来源：http://eos.yj202588.top

TS:   process.exit(1)
来源：http://vjt.birdmap.top

Java: System.exit(1)
来源：http://svn.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://ogg.svipenyu.cn

Ruby: exit 1
来源：http://lea.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zmj.jlsjyb.cn

[M06] 向标准错误输出
来源：http://gzm.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://bel.chenzaomai.com

PHP:  fwrite(STDERR, "err\n");
来源：http://cwm.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://fon.smart0.xyz

TS:   console.error("err")
来源：http://zpg.sweek.top

Java: System.err.println("err")
来源：http://usw.yonumen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xkf.birdmap.top

Ruby: warn "err"
来源：http://mwd.andypj.xyz

C#:   Console.Error.WriteLine("err")
来源：http://iks.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://zsm.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://yel.bbcook.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vbi.xuanzx.com

JS:   require.main === module
来源：http://gjt.hnxiangtu.top

TS:   require.main === module
来源：http://iql.ivvv.top

Java: public static void main(String[] args)
来源：http://uvs.mhx1999.top

Go:   func main()
来源：http://xzw.zhongyouzk.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://llw.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://cia.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://mwm.0kj1m.cn

Py:   platform.system();  platform.python_version()
来源：http://xhr.wangdashe.top

PHP:  PHP_OS;  phpversion();
来源：http://pgc.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://qdo.meibo888.top

TS:   process.platform;  process.version
来源：http://crl.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nar.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://bbf.nanxinkj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ewq.ywan-chungtsiang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://chd.bbcook.cn

================================================================================
来源：http://bsi.yueranfly.top

N. 数据结构与算法
来源：http://fnh.birdmap.top

================================================================================
来源：http://rwo.zhixingplan.top

[N01] 二分查找（有序数组）
来源：http://nhi.yj20258.top

Py:   bisect.bisect_left(arr, x)
来源：http://iuz.hcnkem.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jnp.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://azq.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lpg.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://ehz.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://xdg.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nby.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://mck.cucudq.cn

[N02] 排序（工程实践用内置实现）
来源：http://smi.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://nhx.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qxf.cdnleiting.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hvm.quarkkingdee.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uoy.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mbk.gzhubu.top

Go:   slices.Sort(arr)
来源：http://qak.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://wji.hammf.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iat.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://ttc.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jot.jiagoushi.top

PHP:  // 递归实现，或用 usort
来源：http://weu.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ljj.guannengcc.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xgs.hammf.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://djb.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lvv.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fyj.redwolf501.top

C#:   // 手写递归，或 Array.Sort
来源：http://pbo.havefunace.top

[N04] 斐波那契数列
来源：http://xtg.hnxiangtu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pdb.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sbp.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fhu.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gzp.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iqq.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lwi.hesvh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fsu.yanxiufei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dcy.xziqi.cn

[N05] 最大公约数
来源：http://mar.wangdashe.top

Py:   math.gcd(a, b)
来源：http://nhi.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uwi.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bmd.gotoacloud.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qts.yonumen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mqr.daxiang520.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hig.fengsongda.top

Ruby: a.gcd(b)
来源：http://yts.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yzk.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://far.vqdsnc.cn

Py:   s == s[::-1]
来源：http://azp.xylfe.cn

PHP:  $s === strrev($s);
来源：http://kab.birdmap.top

JS:   s === [...s].reverse().join("")
来源：http://vwk.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://opk.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vec.zhijiandao.cn

Go:   // 双指针从两端比较
来源：http://lvp.tanke756.top


<!-- 参考信息 -->