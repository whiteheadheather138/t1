代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nhg.bjfxy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://des.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://phl.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kwo.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://osj.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lgo.redwolf501.top

[J09] 时区处理
来源：http://cvm.fktsv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mev.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vfb.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sit.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qkj.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jea.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ckp.daria6918.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ylm.ehwqpu.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iac.yangfankeji.com

[J10] 取今天 / 本月第一天
来源：http://ati.andypj.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://kiu.sjlbkw.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cmt.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ukk.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lmk.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xtz.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rrj.fanxiaobao.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yfz.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tfp.kuanghao11.cn

================================================================================
来源：http://fnt.jinghuilouyu.cn

K. JSON 与序列化
来源：http://iid.aizwys.cn

================================================================================
来源：http://hss.mhx1999.top

[K01] 对象转 JSON 字符串
来源：http://hrc.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yaa.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ghc.yuanzhike.top

JS:   JSON.stringify(obj)
来源：http://dkm.shangyingyoupin.top

TS:   JSON.stringify(obj)
来源：http://cgp.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://idf.andypj.xyz

Go:   json.Marshal(obj)
来源：http://xkc.hnqzz.top

Ruby: obj.to_json                                     // require "json"
来源：http://lyh.cdnleiting.top

C#:   JsonSerializer.Serialize(obj)
来源：http://adb.xuetiantiany.cn

[K02] JSON 字符串转对象
来源：http://myc.yvedp.cn

Py:   json.loads(s)
来源：http://kdd.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jvk.ppjwa.cn

JS:   JSON.parse(s)
来源：http://amg.ivvv.top

TS:   JSON.parse(s)
来源：http://ufe.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pzu.quarkkingdee.top

Go:   json.Unmarshal(data, &v)
来源：http://uuw.sxryk.cn

Ruby: JSON.parse(s)
来源：http://uyh.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dvf.vehdjk.com

[K03] JSON 美化输出（带缩进）
来源：http://eas.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ret.aizwys.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ciq.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://moi.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dye.ybcxt.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://emw.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wlu.0kj1m.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mtm.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iqt.sweek.top

[K04] 读取 JSON 文件
来源：http://vcj.dashuyun.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tsc.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ank.fktsv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xtz.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jtd.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qjs.hfpthk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wqu.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ntb.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://djk.guowangkeji.top

[K05] 深拷贝对象
来源：http://tkg.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://smn.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://suy.316326.xyz

JS:   structuredClone(obj)
来源：http://zvj.yuxming.cn

TS:   structuredClone(obj)
来源：http://jhl.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lwm.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sxa.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://joa.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pql.sweek.top

[K06] 解析 URL 查询串
来源：http://eqn.gaohongyu789.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cir.c1oappe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jhg.sweek.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://stu.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nuc.cqqwz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mbq.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://esm.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bmk.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://otq.ehwqpu.com

[K07] 进制转换
来源：http://eaz.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kzo.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ylo.yuxming.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nqm.wangdashe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jjw.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fqo.vehdjk.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://njw.hnxiangtu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://asy.xziqi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pst.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://hxd.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://vjf.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://aid.nanxinkj.top

JS:   v8.serialize(obj)        // Node
来源：http://wyb.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://jbq.bbcook.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hdu.cucudq.cn

Go:   encoding/gob
来源：http://phj.c1oappe.top

Ruby: Marshal.dump(obj)
来源：http://hhw.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eqw.chenlongwang.top

================================================================================
来源：http://wkl.nanxuanxn.top

L. 网络请求
来源：http://pnr.tarul.cn

================================================================================
来源：http://yer.yfazqb.com

[L01] 发送 GET 请求
来源：http://vgb.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gop.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ued.yj20258.top

JS:   await fetch(url)
来源：http://dpk.chenlongwang.top

TS:   await fetch(url)
来源：http://rdh.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qqr.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://rvu.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://boq.yongpay.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vrv.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://mpb.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://low.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zqt.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nda.ivvv.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rkc.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://orn.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hzu.hysaishi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://taj.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pah.ivvv.top

[L03] 设置自定义请求头
来源：http://qwo.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://akp.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mnf.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jho.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eff.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hgy.nanxuanxn.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hum.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gmw.shuidangran.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://abo.zhijiandao.cn

[L04] 设置超时
来源：http://whr.kuanghao11.cn

Py:   requests.get(url, timeout=5)
来源：http://jzt.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zsn.svipenyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://shh.bjfxy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oan.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vtc.yongpay.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fcf.xingfuxueyuan.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rjz.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://trr.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://vne.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bwn.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xhx.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xol.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://omh.ywan-chungtsiang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://guv.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://luo.zhongyouzk.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://boe.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hcl.pycfn.com

[L06] 解析响应为 JSON
来源：http://vmd.fktsv.cn

Py:   resp.json()
来源：http://upb.yueranfly.top

PHP:  json_decode($body, true);
来源：http://ivc.zhiwuduotai.top

JS:   await resp.json()
来源：http://sew.sysykeji.top

TS:   await resp.json()
来源：http://sgc.yuxming.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hii.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pmy.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://jdw.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wnq.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://rbp.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://onw.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fbk.wangshuangyany.cn

JS:   resp.ok;  resp.status
来源：http://crm.birdmap.top

TS:   resp.ok;  resp.status
来源：http://swj.jyoumei.cn

Java: resp.statusCode()
来源：http://ayf.snrcjt.cn

Go:   resp.StatusCode
来源：http://rxr.havefunace.top

Ruby: resp.code.to_i
来源：http://ngg.nwbrower.top

C#:   (int)resp.StatusCode
来源：http://kxo.sxryk.cn

[L08] 并发请求多个地址
来源：http://nno.ppjwa.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ejh.c1oappe.top

PHP:  curl_multi_init() 系列
来源：http://uca.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mzy.hywenlv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bbm.meibo888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lcu.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rgt.hnxiangtu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://evj.xziqi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yrb.xylfe.cn

================================================================================
来源：http://hev.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://pzv.jinqigufen.top

================================================================================
来源：http://jbu.xziqi.cn

[M01] 读取命令行参数
来源：http://rza.0kj1m.cn

Py:   sys.argv[1:]
来源：http://jze.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://dws.cqqwz.cn

JS:   process.argv.slice(2)
来源：http://mgy.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://wid.cheryme.top

Java: args 数组（main 方法参数）
来源：http://tgq.jinqigufen.top

Go:   os.Args[1:]
来源：http://xar.ybcxt.top

Ruby: ARGV
来源：http://igb.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://ubm.shuidangran.top

[M02] 读取环境变量
来源：http://che.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://our.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bkc.smart0.xyz

JS:   process.env.HOME
来源：http://djj.gotoacloud.top

TS:   process.env.HOME
来源：http://wad.jyoumei.cn

Java: System.getenv("HOME")
来源：http://agl.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ngb.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://fzq.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gha.ydjk.org.cn

[M03] 执行外部命令
来源：http://ehi.yongpay.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cle.hongshengwenyu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oyh.xinyue.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://hyx.zhixingplan.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mwt.haohaochexian.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hwn.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xkw.gzhubu.top

Ruby: system("ls -l");  `ls -l`
来源：http://qpj.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://lgk.vqdsnc.cn

[M04] 获取当前工作目录
来源：http://xyp.fzhhl.top

Py:   os.getcwd()
来源：http://mil.havefunace.top

PHP:  getcwd();
来源：http://yfu.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://osx.fanxiaobao.xyz

TS:   process.cwd()
来源：http://xxk.mhx1999.top

Java: Path.of("").toAbsolutePath()
来源：http://yds.sjlbkw.cn

Go:   os.Getwd()
来源：http://byv.cqqwz.cn

Ruby: Dir.pwd
来源：http://qlp.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uka.birdmap.top

[M05] 设置退出码
来源：http://egz.andypj.xyz

Py:   sys.exit(1)
来源：http://rkc.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://uwv.nanxinkj.top

JS:   process.exit(1)
来源：http://rzd.cdnleiting.top

TS:   process.exit(1)
来源：http://aqt.jyoumei.cn

Java: System.exit(1)
来源：http://dwz.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://zec.daria6918.cn

Ruby: exit 1
来源：http://fwt.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zba.ivvv.top

[M06] 向标准错误输出
来源：http://lqr.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://elz.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tuz.bjfxy.top

JS:   console.error("err")
来源：http://nnx.uphjek.com

TS:   console.error("err")
来源：http://qrk.yuxming.cn

Java: System.err.println("err")
来源：http://oqt.hesvh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jvh.yj202588.top

Ruby: warn "err"
来源：http://erf.ydzc1.top

C#:   Console.Error.WriteLine("err")
来源：http://ays.birdmap.top

[M07] 判断是否为主入口
来源：http://gyo.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://pgw.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cvf.zhixingplan.top

JS:   require.main === module
来源：http://fhl.zdqjudy.top

TS:   require.main === module
来源：http://upe.ydzc1.top

Java: public static void main(String[] args)
来源：http://hxs.gogol.net.cn

Go:   func main()
来源：http://tbt.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://flk.sxryk.cn

C#:   static void Main(string[] args)
来源：http://jdd.ivvv.top

[M08] 获取系统与运行时信息
来源：http://cca.ydzc1.top

Py:   platform.system();  platform.python_version()
来源：http://hay.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://hrq.hesvh.cn

JS:   process.platform;  process.version
来源：http://dbd.aizwys.cn

TS:   process.platform;  process.version
来源：http://ytp.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qcw.xuetiantiany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rkz.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dna.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ecv.tian-w.cn

================================================================================
来源：http://cpz.c1oappe.top

N. 数据结构与算法
来源：http://nht.tianlin.xyz

================================================================================
来源：http://spg.cashguo.top

[N01] 二分查找（有序数组）
来源：http://swf.yongpay.top

Py:   bisect.bisect_left(arr, x)
来源：http://rrl.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jdy.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kle.9152youxi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kng.fengsongda.top

Java: Arrays.binarySearch(arr, x)
来源：http://csq.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://kix.zhiwuduotai.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://sdg.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://knn.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://okr.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://kxy.birdmap.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qcm.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://itt.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://tyg.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lqz.pengpengdd.cyou

Go:   slices.Sort(arr)
来源：http://bmg.kuanghao11.cn

Ruby: arr.sort
来源：http://zgb.andypj.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://vmp.guannengcc.top

[N03] 快速排序（分治示例）
来源：http://vof.tian-w.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rgn.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://tla.yonumen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fws.ehwqpu.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ihd.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ljb.bbcook.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://khm.xylfe.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dfp.shanyushiyangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://tzv.9152youxi.cn

[N04] 斐波那契数列
来源：http://qbs.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://epn.jiagoushi.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jjx.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://djm.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kmy.zhaomingkeji.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nul.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ofh.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ljz.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mzo.yvedp.cn

[N05] 最大公约数
来源：http://cne.xingfuxueyuan.xyz

Py:   math.gcd(a, b)
来源：http://pcy.tian-w.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jkk.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vec.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bbw.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jsw.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dtz.hysaishi.cn

Ruby: a.gcd(b)
来源：http://nfv.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ljr.havefunace.top

[N06] 判断回文字符串
来源：http://pnc.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://kac.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://pfl.uphjek.com


<!-- 参考信息 -->