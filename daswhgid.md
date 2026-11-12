代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://wzl.bjfxy.top

[J08] 提取年月日与星期
来源：http://qed.yfazqb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://emt.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oph.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fxa.zhoulong.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gyx.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hoj.yonumen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://btn.wangshuangyany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qbp.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://unf.shuidangran.top

[J09] 时区处理
来源：http://woy.sysykeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bpd.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://msg.cashguo.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jgj.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vec.yj20258888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xwz.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vuy.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://lkg.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qys.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://llo.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xsb.feifeiyinyue.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bnf.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rsr.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wjw.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dsz.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pku.sweek.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fiw.0kj1m.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wpy.fengsongda.top

================================================================================
来源：http://rtt.zhiwuduotai.top

K. JSON 与序列化
来源：http://kgz.yueranfly.top

================================================================================
来源：http://kqo.guannengcc.top

[K01] 对象转 JSON 字符串
来源：http://xys.redwolf501.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qum.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qwx.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://atc.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://dev.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://isj.fengsongda.top

Go:   json.Marshal(obj)
来源：http://xgf.aibaodan.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ryb.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lad.haohaochexian.top

[K02] JSON 字符串转对象
来源：http://kyj.svipenyu.cn

Py:   json.loads(s)
来源：http://dsv.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nwj.shanyushiyangtech.top

JS:   JSON.parse(s)
来源：http://xgz.jiagoushi.top

TS:   JSON.parse(s)
来源：http://rxp.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://irs.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://lvq.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://xva.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zjh.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://egt.yj20258.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kbo.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://orn.nwbrower.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tur.aizwys.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ygl.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pxa.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xjd.wangshuangyany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jaz.ybcxt.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ffi.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://dts.nanxuanxn.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lgq.c1oappe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://idi.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ywt.zycfv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ofp.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vyu.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xcp.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ukz.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uyp.ydjk.org.cn

[K05] 深拷贝对象
来源：http://dfd.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://emz.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://pwr.nwbrower.top

JS:   structuredClone(obj)
来源：http://ncs.xylfe.cn

TS:   structuredClone(obj)
来源：http://xne.fzhhl.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sfr.ppjwa.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ybu.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oev.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pxh.hammf.cn

[K06] 解析 URL 查询串
来源：http://bfx.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kau.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://der.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wmn.guannengcc.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jwr.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hlx.chenjidiqi.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://ssr.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pnj.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aze.shzxlz.cn

[K07] 进制转换
来源：http://muo.jinyuanbaomall.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bml.yangfankeji.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xjy.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iuo.nwbrower.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hwk.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wxt.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://soy.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qcn.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nff.jiagoushi.top

[K08] 二进制序列化（非 JSON）
来源：http://bdj.meibo888.top

Py:   pickle.dumps(obj)
来源：http://hgl.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cbh.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://pyj.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ult.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gld.ivvv.top

Go:   encoding/gob
来源：http://grc.feifeiyinyue.top

Ruby: Marshal.dump(obj)
来源：http://ajf.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zej.fzhhl.top

================================================================================
来源：http://wau.redwolf501.top

L. 网络请求
来源：http://bqs.hnqzz.top

================================================================================
来源：http://ntj.yvedp.cn

[L01] 发送 GET 请求
来源：http://ygf.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://trb.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zdl.tianlin.xyz

JS:   await fetch(url)
来源：http://kio.yuxming.cn

TS:   await fetch(url)
来源：http://lfa.yonumen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vbo.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://cvf.tarul.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yym.cdnleiting.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zmp.xuanzx.com

[L02] 发送 POST JSON
来源：http://syk.gogol.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://esk.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mtd.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zzp.yj202588.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://esg.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lqp.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://khh.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ccw.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://spu.jiagoushi.top

[L03] 设置自定义请求头
来源：http://tbq.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yjf.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iir.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lit.aibaodan.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bsx.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ntr.chenzaomai.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xft.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fvv.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mcj.ywan-chungtsiang.top

[L04] 设置超时
来源：http://tgu.xuetiantiany.cn

Py:   requests.get(url, timeout=5)
来源：http://mgv.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ovu.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sev.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dcv.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ryy.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wzf.sweek.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pvu.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tke.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://quh.sjlbkw.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ivj.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sgk.52xcode.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gvi.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kul.sxryk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gya.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://akp.nanxuanxn.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fqj.guowangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xqt.guannengcc.top

[L06] 解析响应为 JSON
来源：http://ury.redwolf501.top

Py:   resp.json()
来源：http://ujd.meibo888.top

PHP:  json_decode($body, true);
来源：http://gms.jqgfzy.top

JS:   await resp.json()
来源：http://tfe.havefunace.top

TS:   await resp.json()
来源：http://kmd.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mlv.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qnv.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://gla.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ufr.yuxming.cn

[L07] 处理 HTTP 状态码
来源：http://aqj.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://onf.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://akh.sysykeji.top

JS:   resp.ok;  resp.status
来源：http://fhh.yj20258.top

TS:   resp.ok;  resp.status
来源：http://jah.shangyingyoupin.top

Java: resp.statusCode()
来源：http://vdm.nanxinkj.top

Go:   resp.StatusCode
来源：http://lga.nwbrower.top

Ruby: resp.code.to_i
来源：http://onp.yfazqb.com

C#:   (int)resp.StatusCode
来源：http://adb.jinqigufen.top

[L08] 并发请求多个地址
来源：http://jvk.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tsx.yangfankeji.com

PHP:  curl_multi_init() 系列
来源：http://hif.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rsn.yfazqb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ahp.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sdc.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bhp.jinghuilouyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mwz.jiagoushi.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wxu.chenjidiqi.icu

================================================================================
来源：http://xqw.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://cxy.sufxvd.cn

================================================================================
来源：http://bxi.kuanghao11.cn

[M01] 读取命令行参数
来源：http://bra.hnxiangtu.top

Py:   sys.argv[1:]
来源：http://zkc.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://poq.jlsjyb.cn

JS:   process.argv.slice(2)
来源：http://lid.andypj.xyz

TS:   process.argv.slice(2)
来源：http://hba.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://jut.daria6918.cn

Go:   os.Args[1:]
来源：http://soo.daria6918.cn

Ruby: ARGV
来源：http://wpv.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://sed.feifeiyinyue.top

[M02] 读取环境变量
来源：http://pgh.cucudq.cn

Py:   os.environ.get("HOME")
来源：http://yqh.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vmh.xinyue.icu

JS:   process.env.HOME
来源：http://bdo.xuetiantiany.cn

TS:   process.env.HOME
来源：http://ety.haohaochexian.top

Java: System.getenv("HOME")
来源：http://aqz.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vnk.yvedp.cn

Ruby: ENV["HOME"]
来源：http://onv.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zrv.sysykeji.top

[M03] 执行外部命令
来源：http://mac.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xac.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kqx.havefunace.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mks.jyoumei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lvc.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gjs.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://fbx.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://cre.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://glr.shuidangran.top

[M04] 获取当前工作目录
来源：http://way.ppjwa.cn

Py:   os.getcwd()
来源：http://wbj.tianlin.xyz

PHP:  getcwd();
来源：http://djq.dianchejie.cn

JS:   process.cwd()
来源：http://wrp.dashuyun.cn

TS:   process.cwd()
来源：http://rot.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://dac.daria6918.cn

Go:   os.Getwd()
来源：http://tpc.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://ukc.daria6918.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lfp.fzhhl.top

[M05] 设置退出码
来源：http://jxv.meibo888.top

Py:   sys.exit(1)
来源：http://rvk.sufxvd.cn

PHP:  exit(1);
来源：http://skr.jqgfzy.top

JS:   process.exit(1)
来源：http://bhv.ppjwa.cn

TS:   process.exit(1)
来源：http://pam.shuidangran.top

Java: System.exit(1)
来源：http://cyw.smart0.xyz

Go:   os.Exit(1)
来源：http://prt.sjlbkw.cn

Ruby: exit 1
来源：http://kom.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mmy.tianlin.xyz

[M06] 向标准错误输出
来源：http://xrg.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://wsd.shanyushiyangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pha.fktsv.cn

JS:   console.error("err")
来源：http://bsb.chenzaomai.com

TS:   console.error("err")
来源：http://zjb.yuxming.cn

Java: System.err.println("err")
来源：http://bge.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ofe.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://hwz.hnqzz.top

C#:   Console.Error.WriteLine("err")
来源：http://sfu.sysykeji.top

[M07] 判断是否为主入口
来源：http://pjh.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://jiq.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jll.bjfxy.top

JS:   require.main === module
来源：http://xdd.snrcjt.cn

TS:   require.main === module
来源：http://pbc.vehdjk.com

Java: public static void main(String[] args)
来源：http://tiw.hnxiangtu.top

Go:   func main()
来源：http://ynr.jinyuanbaomall.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cla.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://nef.iojbl.cn

[M08] 获取系统与运行时信息
来源：http://hls.daria6918.cn

Py:   platform.system();  platform.python_version()
来源：http://fwn.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://aja.cucudq.cn

JS:   process.platform;  process.version
来源：http://crw.gaohongyu789.top

TS:   process.platform;  process.version
来源：http://djw.52xcode.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xxt.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://xyy.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://avw.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tgw.jinqigfzy.top

================================================================================
来源：http://axm.fengsongda.top

N. 数据结构与算法
来源：http://wvy.vehdjk.com

================================================================================
来源：http://dld.tarul.cn

[N01] 二分查找（有序数组）
来源：http://bnr.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://czj.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qey.jinqigufen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pyv.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://utq.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://agv.fktsv.cn

Go:   sort.SearchInts(arr, x)
来源：http://rzy.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hgk.yonumen.top

C#:   Array.BinarySearch(arr, x)
来源：http://akr.yongpay.top

[N02] 排序（工程实践用内置实现）
来源：http://igi.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://pwq.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://weh.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rpf.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://acg.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://veh.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://zgx.yuanzhike.top

Ruby: arr.sort
来源：http://iha.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xet.zhixingplan.top

[N03] 快速排序（分治示例）
来源：http://pgz.hesvh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bwh.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://fev.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rdq.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xxp.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sal.wangdashe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mtz.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tue.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://bjt.daria6918.cn

[N04] 斐波那契数列
来源：http://ecz.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ahu.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xxe.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qjl.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://htv.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gls.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kup.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vue.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zdg.9152youxi.cn

[N05] 最大公约数
来源：http://sbl.316326.xyz

Py:   math.gcd(a, b)
来源：http://vbp.hnqzz.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uov.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://apm.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qvv.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://slu.ywan-chungtsiang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://okh.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://pue.yfazqb.com


<!-- 参考信息 -->