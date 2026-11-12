代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://ihp.ydzc1.top

[J08] 提取年月日与星期
来源：http://rpa.hywenlv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ewf.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xhh.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gtq.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://efl.aizwys.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ghl.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://seu.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://syg.gogol.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rve.cashguo.top

[J09] 时区处理
来源：http://lhr.iojbl.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kge.guannengcc.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fiz.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tkp.cheryme.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jsv.zdqjudy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jyy.xylfe.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://unr.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qsk.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://edt.sufxvd.cn

[J10] 取今天 / 本月第一天
来源：http://hgg.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dkf.cashguo.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dxl.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nlw.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rct.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rqn.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cti.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vxe.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://duy.hcnkem.com

================================================================================
来源：http://jks.fehbvm.com

K. JSON 与序列化
来源：http://kgu.jianghu66.top

================================================================================
来源：http://bcp.sweek.top

[K01] 对象转 JSON 字符串
来源：http://oiu.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zsv.jyoumei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uhg.pycfn.com

JS:   JSON.stringify(obj)
来源：http://sae.birdmap.top

TS:   JSON.stringify(obj)
来源：http://bgq.yvedp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lyf.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://ojv.andypj.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://qdy.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://pgx.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://mcz.jiagoushi.top

Py:   json.loads(s)
来源：http://apy.nwbrower.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wht.daria6918.cn

JS:   JSON.parse(s)
来源：http://hsb.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://mnp.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qfg.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://khv.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://lic.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sqa.andypj.xyz

[K03] JSON 美化输出（带缩进）
来源：http://ork.gzhubu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lqg.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vzd.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kzn.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://frn.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cdf.snrcjt.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qkc.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bdh.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xhu.cashguo.top

[K04] 读取 JSON 文件
来源：http://ffy.hywenlv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jrq.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mzo.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xyj.smart0.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ymc.zhixingplan.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://krn.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zwl.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uwd.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zau.yfazqb.com

[K05] 深拷贝对象
来源：http://rni.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://xyq.yuanzhike.top

PHP:  unserialize(serialize($obj));
来源：http://fty.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://snt.aibaodan.cn

TS:   structuredClone(obj)
来源：http://fnt.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rby.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://por.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vpw.nanxinkj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ags.sufxvd.cn

[K06] 解析 URL 查询串
来源：http://rda.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cbw.meibo888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ajq.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pdr.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qhe.redwolf501.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oqu.iojbl.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nah.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xag.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dot.jyoumei.cn

[K07] 进制转换
来源：http://hjl.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rce.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oxf.daxiang520.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wrt.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://aml.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://edu.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qvf.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://phl.smart0.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sgm.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://kot.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://djz.zdbjq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tjz.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://bsw.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://yll.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lfg.sweek.top

Go:   encoding/gob
来源：http://iyh.yangfankeji.com

Ruby: Marshal.dump(obj)
来源：http://cgc.cqqwz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bcb.guannengcc.top

================================================================================
来源：http://xwt.ywan-chungtsiang.top

L. 网络请求
来源：http://ule.tian-w.cn

================================================================================
来源：http://uog.sweek.top

[L01] 发送 GET 请求
来源：http://jyv.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://grp.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fjw.zycfv.cn

JS:   await fetch(url)
来源：http://tby.yongpay.top

TS:   await fetch(url)
来源：http://qrb.tarul.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ops.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://pkw.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hkl.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kuq.tarul.cn

[L02] 发送 POST JSON
来源：http://czf.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://igd.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gsm.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://adi.meibo888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://crm.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wob.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nyn.hammf.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yah.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://abt.guannengcc.top

[L03] 设置自定义请求头
来源：http://clg.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jkz.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://riq.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dnd.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hxd.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hqe.sysykeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bso.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qge.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eby.quarkkingdee.top

[L04] 设置超时
来源：http://zht.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://xhq.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zfu.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gxd.guannengcc.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://moq.sjlbkw.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kuw.xylfe.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hbw.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nhw.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://knv.jqgfzy.top

[L05] 上传文件（multipart）
来源：http://wkl.shzxlz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://usj.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fvm.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ish.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jxr.yangfankeji.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sto.xziqi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iny.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fdt.mhx1999.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bry.guannengcc.top

[L06] 解析响应为 JSON
来源：http://qao.smart0.xyz

Py:   resp.json()
来源：http://sbe.jqgfzy.top

PHP:  json_decode($body, true);
来源：http://nzu.cqqwz.cn

JS:   await resp.json()
来源：http://hqs.mhx1999.top

TS:   await resp.json()
来源：http://kzq.gaohongyu789.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://noj.zycfv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jqg.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://rwd.quarkkingdee.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wam.chenlongwang.top

[L07] 处理 HTTP 状态码
来源：http://enj.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fdc.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cgx.aizwys.cn

JS:   resp.ok;  resp.status
来源：http://bwt.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://qml.cdnleiting.top

Java: resp.statusCode()
来源：http://yhx.yuanzhike.top

Go:   resp.StatusCode
来源：http://mrs.aizwys.cn

Ruby: resp.code.to_i
来源：http://xqm.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://yjz.zhixingplan.top

[L08] 并发请求多个地址
来源：http://ljv.redwolf501.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oke.bjfxy.top

PHP:  curl_multi_init() 系列
来源：http://iwa.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://opy.hfpthk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hkw.sxryk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pxk.zhengqikj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hlh.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uzj.jqgfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zmg.daxiang520.top

================================================================================
来源：http://vsl.quarkkingdee.top

M. 命令行 / 进程 / 环境
来源：http://acu.bjfxy.top

================================================================================
来源：http://vxg.jianghu66.top

[M01] 读取命令行参数
来源：http://bcu.cdnleiting.top

Py:   sys.argv[1:]
来源：http://qwc.cucudq.cn

PHP:  $argv;  $argc;
来源：http://czs.kuanghao11.cn

JS:   process.argv.slice(2)
来源：http://knp.aibaodan.cn

TS:   process.argv.slice(2)
来源：http://gvm.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://qmi.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://fok.c1oappe.top

Ruby: ARGV
来源：http://osk.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://tlg.haohaochexian.top

[M02] 读取环境变量
来源：http://cof.0kj1m.cn

Py:   os.environ.get("HOME")
来源：http://ldb.ydjk.org.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vmr.jiagoushi.top

JS:   process.env.HOME
来源：http://awq.kuanghao11.cn

TS:   process.env.HOME
来源：http://rtb.mhx1999.top

Java: System.getenv("HOME")
来源：http://six.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qqt.yongpay.top

Ruby: ENV["HOME"]
来源：http://iby.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sbi.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://aqe.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eya.hysaishi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dka.ppjwa.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kkm.zhaomingkeji.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://rvn.ybcxt.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zof.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://bas.jyoumei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pii.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://txv.jyoumei.cn

[M04] 获取当前工作目录
来源：http://qlo.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://hvi.hnxiangtu.top

PHP:  getcwd();
来源：http://uns.sweek.top

JS:   process.cwd()
来源：http://ikb.shuidangran.top

TS:   process.cwd()
来源：http://nah.shuidangran.top

Java: Path.of("").toAbsolutePath()
来源：http://oze.zycfv.cn

Go:   os.Getwd()
来源：http://zhw.zhixingplan.top

Ruby: Dir.pwd
来源：http://pne.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ouk.yuxming.cn

[M05] 设置退出码
来源：http://spe.cdnleiting.top

Py:   sys.exit(1)
来源：http://xzy.shzxlz.cn

PHP:  exit(1);
来源：http://lxw.ybcxt.top

JS:   process.exit(1)
来源：http://csp.sxryk.cn

TS:   process.exit(1)
来源：http://izx.bjfxy.top

Java: System.exit(1)
来源：http://woe.sysykeji.top

Go:   os.Exit(1)
来源：http://ofe.zhongyouzk.top

Ruby: exit 1
来源：http://ooq.9152youxi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nrt.sxryk.cn

[M06] 向标准错误输出
来源：http://dbg.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://xpk.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xrd.jinghuilouyu.cn

JS:   console.error("err")
来源：http://rdm.zycfv.cn

TS:   console.error("err")
来源：http://veu.zdqjudy.top

Java: System.err.println("err")
来源：http://ngg.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fct.andypj.xyz

Ruby: warn "err"
来源：http://wdh.guannengcc.top

C#:   Console.Error.WriteLine("err")
来源：http://ruy.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://vau.zdqjudy.top

Py:   if __name__ == "__main__":
来源：http://gnf.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tyo.xuetiantiany.cn

JS:   require.main === module
来源：http://zpc.hesvh.cn

TS:   require.main === module
来源：http://yne.yvedp.cn

Java: public static void main(String[] args)
来源：http://buz.tarul.cn

Go:   func main()
来源：http://uwy.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zdv.uphjek.com

C#:   static void Main(string[] args)
来源：http://ejq.yongpay.top

[M08] 获取系统与运行时信息
来源：http://wih.fktsv.cn

Py:   platform.system();  platform.python_version()
来源：http://dcm.epnwcf.com

PHP:  PHP_OS;  phpversion();
来源：http://ioa.ivvv.top

JS:   process.platform;  process.version
来源：http://bpb.daria6918.cn

TS:   process.platform;  process.version
来源：http://bhv.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fkr.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uor.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zwo.hongshengwenyu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ivw.fehbvm.com

================================================================================
来源：http://hip.jianghu66.top

N. 数据结构与算法
来源：http://olj.52xcode.cn

================================================================================
来源：http://pwv.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://xwu.chenlongwang.top

Py:   bisect.bisect_left(arr, x)
来源：http://wvu.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://whg.xingfuxueyuan.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lzm.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://diy.0kj1m.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mmu.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://waq.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://eyr.gogol.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rns.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://fcg.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://rzb.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jad.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://tut.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://her.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yay.cashguo.top

Go:   slices.Sort(arr)
来源：http://omj.ivvv.top

Ruby: arr.sort
来源：http://wau.gzhubu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xto.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://djk.zhoulong.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ufq.aizwys.cn

PHP:  // 递归实现，或用 usort
来源：http://fna.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ndr.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ots.haohaochexian.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pgu.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nir.hnqzz.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://inb.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bpa.redwolf501.top

[N04] 斐波那契数列
来源：http://mio.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jiy.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qrb.zdqjudy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sba.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yvn.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gtg.fengsongda.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yme.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wqq.iojbl.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gxn.shuidangran.top

[N05] 最大公约数
来源：http://uql.birdmap.top

Py:   math.gcd(a, b)
来源：http://ddj.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pkl.shzxlz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://huw.zhijiandao.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xjd.cucudq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ymy.guannengcc.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://igx.tarul.cn

Ruby: a.gcd(b)
来源：http://kvs.dianchejie.cn


<!-- 参考信息 -->