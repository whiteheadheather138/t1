代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uwu.xylfe.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bfp.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xte.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://dvb.bbcook.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://olq.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://asr.jinyuanbaomall.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lqu.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gsr.kuanghao11.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uyt.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xyk.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eip.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zhz.tarul.cn

================================================================================
来源：http://tgf.yuanzhike.top

K. JSON 与序列化
来源：http://aiy.chenjidiqi.icu

================================================================================
来源：http://ohd.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://rrx.jinqigfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ivr.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tsf.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://upy.nanxinkj.top

TS:   JSON.stringify(obj)
来源：http://zpe.sweek.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tit.cqqwz.cn

Go:   json.Marshal(obj)
来源：http://hwt.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zfp.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oyx.yanxiufei.cn

[K02] JSON 字符串转对象
来源：http://rpy.guowangkeji.top

Py:   json.loads(s)
来源：http://fsr.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fvt.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://jyj.guannengcc.top

TS:   JSON.parse(s)
来源：http://xmq.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fsm.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://fmv.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://sde.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://daw.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://wzi.gaohongyu789.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ppf.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://itb.nwbrower.top

JS:   JSON.stringify(obj, null, 2)
来源：http://txx.yj20258888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bgu.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rcl.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gmh.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lup.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ksc.sjlbkw.cn

[K04] 读取 JSON 文件
来源：http://adx.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gqa.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hwm.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://but.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gtm.jinghuilouyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kvv.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vtd.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yyf.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gsd.zdbjq.cn

[K05] 深拷贝对象
来源：http://ubl.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://iqu.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://qmk.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://tkd.c1oappe.top

TS:   structuredClone(obj)
来源：http://xbi.wangdashe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xnd.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nqj.jinqigufen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nsb.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ytb.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://fbe.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mlf.ppjwa.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bit.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hxl.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rkx.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sqe.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ona.daxiang520.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wlw.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pnw.ywan-chungtsiang.top

[K07] 进制转换
来源：http://dvr.sweek.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://clz.mhx1999.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cin.yfazqb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vhj.fengsongda.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vqu.xuetiantiany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zza.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nwx.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lep.hesvh.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://znn.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://bjp.zhixingplan.top

Py:   pickle.dumps(obj)
来源：http://wcg.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dpw.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://ntg.chenzaomai.com

TS:   v8.serialize(obj)        // Node
来源：http://rcq.havefunace.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dts.haohaochexian.top

Go:   encoding/gob
来源：http://hzt.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://hjl.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ueo.zhaomingkeji.xyz

================================================================================
来源：http://njh.epnwcf.com

L. 网络请求
来源：http://eff.dashuyun.cn

================================================================================
来源：http://qce.shzxlz.cn

[L01] 发送 GET 请求
来源：http://ycc.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pqi.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://spj.zdqjudy.top

JS:   await fetch(url)
来源：http://upp.cdnleiting.top

TS:   await fetch(url)
来源：http://buz.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mkw.yfazqb.com

Go:   resp, err := http.Get(url)
来源：http://gkb.bbcook.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pyz.hesvh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hmd.cashguo.top

[L02] 发送 POST JSON
来源：http://pdf.zhiwuduotai.top

Py:   requests.post(url, json={"a": 1})
来源：http://qay.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fmt.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://whm.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zcw.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://udx.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dvx.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gxb.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sqs.jqgfzy.top

[L03] 设置自定义请求头
来源：http://bbo.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kth.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tlf.iojbl.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jnt.shanyushiyangtech.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nzs.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uxm.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qbc.xingfuxueyuan.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ehn.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ymc.fengsongda.top

[L04] 设置超时
来源：http://vsr.zdqjudy.top

Py:   requests.get(url, timeout=5)
来源：http://rdj.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://riv.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kjt.guowangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fdr.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qur.fanxiaobao.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rhn.zhengqikj.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dae.sufxvd.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://syg.yvedp.cn

[L05] 上传文件（multipart）
来源：http://wbm.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ium.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uie.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fqj.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dzd.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://crd.jiagoushi.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lpy.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://seo.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iwc.tarul.cn

[L06] 解析响应为 JSON
来源：http://sjv.jinyuanbaomall.cn

Py:   resp.json()
来源：http://nbd.snrcjt.cn

PHP:  json_decode($body, true);
来源：http://uoa.vqdsnc.cn

JS:   await resp.json()
来源：http://kpd.ydjk.org.cn

TS:   await resp.json()
来源：http://gbj.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xpg.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gsg.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://ktc.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sqx.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://xca.jianghu66.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qot.hysaishi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://txl.fanxiaobao.xyz

JS:   resp.ok;  resp.status
来源：http://xps.ybcxt.top

TS:   resp.ok;  resp.status
来源：http://unn.kuanghao11.cn

Java: resp.statusCode()
来源：http://qbn.yueranfly.top

Go:   resp.StatusCode
来源：http://gwm.aibaodan.cn

Ruby: resp.code.to_i
来源：http://maw.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://yyl.fengsongda.top

[L08] 并发请求多个地址
来源：http://yvz.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kup.chenzaomai.com

PHP:  curl_multi_init() 系列
来源：http://xhm.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vsh.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gws.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://obd.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fzl.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ewz.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eph.yj202588.top

================================================================================
来源：http://zvb.0kj1m.cn

M. 命令行 / 进程 / 环境
来源：http://ddm.kuanghao11.cn

================================================================================
来源：http://lmt.uphjek.com

[M01] 读取命令行参数
来源：http://bwr.0kj1m.cn

Py:   sys.argv[1:]
来源：http://hjr.jqgfzy.top

PHP:  $argv;  $argc;
来源：http://tfp.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://bwk.redwolf501.top

TS:   process.argv.slice(2)
来源：http://jhd.hfpthk.cn

Java: args 数组（main 方法参数）
来源：http://dgb.zhengqikj.top

Go:   os.Args[1:]
来源：http://etw.feifeiyinyue.top

Ruby: ARGV
来源：http://dbw.ppjwa.cn

C#:   args 数组（Main 方法参数）
来源：http://fek.yuxming.cn

[M02] 读取环境变量
来源：http://loz.tanke756.top

Py:   os.environ.get("HOME")
来源：http://zed.jinqigfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yek.chenzaomai.com

JS:   process.env.HOME
来源：http://zev.shangyingyoupin.top

TS:   process.env.HOME
来源：http://mls.hfpthk.cn

Java: System.getenv("HOME")
来源：http://fik.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zpl.yj20258.top

Ruby: ENV["HOME"]
来源：http://fii.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mml.gaohongyu789.top

[M03] 执行外部命令
来源：http://pkg.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gcs.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xvu.tarul.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aqc.jlsjyb.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fhb.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jey.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://khx.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kwt.chenzaomai.com

C#:   Process.Start("ls", "-l");
来源：http://uve.snrcjt.cn

[M04] 获取当前工作目录
来源：http://buh.aibaodan.cn

Py:   os.getcwd()
来源：http://zhz.zhoulong.xyz

PHP:  getcwd();
来源：http://txo.daria6918.cn

JS:   process.cwd()
来源：http://cwh.hnxiangtu.top

TS:   process.cwd()
来源：http://nct.daxiang520.top

Java: Path.of("").toAbsolutePath()
来源：http://zed.hongshengwenyu.top

Go:   os.Getwd()
来源：http://suz.yuanzhike.top

Ruby: Dir.pwd
来源：http://wef.xziqi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ejl.aizwys.cn

[M05] 设置退出码
来源：http://fbs.guowangkeji.top

Py:   sys.exit(1)
来源：http://dve.jinghuilouyu.cn

PHP:  exit(1);
来源：http://wxd.yonumen.top

JS:   process.exit(1)
来源：http://cfw.ehwqpu.com

TS:   process.exit(1)
来源：http://oan.uphjek.com

Java: System.exit(1)
来源：http://nxq.bjfxy.top

Go:   os.Exit(1)
来源：http://svd.ywan-chungtsiang.top

Ruby: exit 1
来源：http://qku.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jhx.redwolf501.top

[M06] 向标准错误输出
来源：http://rxv.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://eee.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ksf.hongshengwenyu.top

JS:   console.error("err")
来源：http://jil.bjfxy.top

TS:   console.error("err")
来源：http://orf.nanxuanxn.top

Java: System.err.println("err")
来源：http://hxu.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://duf.ivvv.top

Ruby: warn "err"
来源：http://cxc.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://swg.andypj.xyz

[M07] 判断是否为主入口
来源：http://niy.zhoulong.xyz

Py:   if __name__ == "__main__":
来源：http://dkg.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vdt.yongpay.top

JS:   require.main === module
来源：http://toq.hnxiangtu.top

TS:   require.main === module
来源：http://hqo.bbcook.cn

Java: public static void main(String[] args)
来源：http://kjr.xziqi.cn

Go:   func main()
来源：http://fpn.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jbq.aizwys.cn

C#:   static void Main(string[] args)
来源：http://dzj.hnxiangtu.top

[M08] 获取系统与运行时信息
来源：http://aun.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://uco.fanxiaobao.xyz

PHP:  PHP_OS;  phpversion();
来源：http://fls.0kj1m.cn

JS:   process.platform;  process.version
来源：http://frc.chenlongwang.top

TS:   process.platform;  process.version
来源：http://qtn.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tyt.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://kig.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ucv.iojbl.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nbp.ivvv.top

================================================================================
来源：http://vib.hfpthk.cn

N. 数据结构与算法
来源：http://vhh.kuanghao11.cn

================================================================================
来源：http://ckt.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://low.cdnleiting.top

Py:   bisect.bisect_left(arr, x)
来源：http://tea.fengsongda.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kzv.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ebe.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rgf.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://pyk.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://tqj.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://wda.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://ked.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://zql.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://gxx.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oem.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fmp.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://aga.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://upq.tarul.cn

Go:   slices.Sort(arr)
来源：http://ppj.yueranfly.top

Ruby: arr.sort
来源：http://pbk.chenlongwang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pqj.sxryk.cn

[N03] 快速排序（分治示例）
来源：http://iqa.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ads.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://frd.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://skl.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iyq.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qlt.52xcode.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fxw.hnxiangtu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mhb.fanxiaobao.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://jji.mhx1999.top

[N04] 斐波那契数列
来源：http://ktg.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vbt.yj202588.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blj.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kkz.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rsk.xziqi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lzm.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qcz.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pqz.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ndk.smart0.xyz

[N05] 最大公约数
来源：http://fpl.aibaodan.cn

Py:   math.gcd(a, b)
来源：http://yvj.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ghk.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://chx.andypj.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dcn.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zfu.tianlin.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qsn.52xcode.cn

Ruby: a.gcd(b)
来源：http://xru.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cdy.pycfn.com

[N06] 判断回文字符串
来源：http://kbo.gogol.net.cn

Py:   s == s[::-1]
来源：http://icg.yongpay.top

PHP:  $s === strrev($s);
来源：http://emx.gaohongyu789.top

JS:   s === [...s].reverse().join("")
来源：http://vko.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://pcf.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gei.tian-w.cn

Go:   // 双指针从两端比较
来源：http://sjj.nwbrower.top

Ruby: s == s.reverse
来源：http://hba.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yjt.yfazqb.com

[N07] 两数之和（返回下标）
来源：http://bff.tianlin.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ueh.ctjpmb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oun.xziqi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rob.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://ftc.vehdjk.com

Java: // 手写 HashMap
来源：http://slm.ehwqpu.com


<!-- 参考信息 -->