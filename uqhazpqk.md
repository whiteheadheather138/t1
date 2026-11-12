代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oxy.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vlg.pengpengdd.cyou

[J09] 时区处理
来源：http://lvp.jinqigufen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://omo.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hfi.daria6918.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xib.zhiwuduotai.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rzi.zdqjudy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bve.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yar.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://djp.ydjk.org.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oct.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://cft.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://mak.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aam.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uxg.xylfe.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kne.guowangkeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vwo.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://chp.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://plq.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mqy.jlsjyb.cn

================================================================================
来源：http://seo.epnwcf.com

K. JSON 与序列化
来源：http://okw.tian-w.cn

================================================================================
来源：http://sxc.sysykeji.top

[K01] 对象转 JSON 字符串
来源：http://drh.iojbl.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ack.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://swz.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://zav.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://afw.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mob.zdqjudy.top

Go:   json.Marshal(obj)
来源：http://ziq.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://fpy.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vom.gogol.net.cn

[K02] JSON 字符串转对象
来源：http://rlz.xingfuxueyuan.xyz

Py:   json.loads(s)
来源：http://jeg.pengpengdd.cyou

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wlg.meibo888.top

JS:   JSON.parse(s)
来源：http://kpc.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://joa.wangshuangyany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://npg.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://ebo.meibo888.top

Ruby: JSON.parse(s)
来源：http://hcv.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zcs.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://ajq.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qrm.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://don.xziqi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zlx.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rnz.52xcode.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fnr.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jpt.yangfankeji.com

Ruby: JSON.pretty_generate(obj)
来源：http://qij.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qaf.gaohongyu789.top

[K04] 读取 JSON 文件
来源：http://abd.daria6918.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ryk.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://whs.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ivx.fengsongda.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vjj.redwolf501.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ybt.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wws.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lco.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cvh.yuanzhike.top

[K05] 深拷贝对象
来源：http://hej.jyoumei.cn

Py:   copy.deepcopy(obj)
来源：http://luo.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://gby.hysaishi.cn

JS:   structuredClone(obj)
来源：http://cqf.zhongyouzk.top

TS:   structuredClone(obj)
来源：http://chn.gogol.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oqt.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pur.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://olm.zdbjq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wgk.wangshuangyany.cn

[K06] 解析 URL 查询串
来源：http://nop.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vxi.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rrn.dashuyun.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cbb.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tdh.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rvl.9152youxi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://npk.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jwu.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hmd.birdmap.top

[K07] 进制转换
来源：http://bof.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ydi.jqgfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ehr.zhiwuduotai.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blp.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ntj.bjfxy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://olw.shuidangran.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iwn.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dse.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ixc.fanxiaobao.xyz

[K08] 二进制序列化（非 JSON）
来源：http://boj.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://keh.hesvh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zui.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://mfg.hfpthk.cn

TS:   v8.serialize(obj)        // Node
来源：http://obt.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hla.tian-w.cn

Go:   encoding/gob
来源：http://yot.smart0.xyz

Ruby: Marshal.dump(obj)
来源：http://psx.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://byn.uphjek.com

================================================================================
来源：http://tns.yuxming.cn

L. 网络请求
来源：http://how.redwolf501.top

================================================================================
来源：http://jti.nanxinkj.top

[L01] 发送 GET 请求
来源：http://yai.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cmq.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pym.daxiang520.top

JS:   await fetch(url)
来源：http://uff.tian-w.cn

TS:   await fetch(url)
来源：http://yht.jianghu66.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ejm.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://eso.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zmt.hesvh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://riu.yueranfly.top

[L02] 发送 POST JSON
来源：http://ngs.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://aex.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://khv.chenlongwang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wxk.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ysl.daria6918.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kko.pengpengdd.cyou

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dtk.fanxiaobao.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jhy.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kqk.nwbrower.top

[L03] 设置自定义请求头
来源：http://fxn.tianlin.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mml.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wuq.dashuyun.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gus.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bxk.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ztg.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nvz.ehwqpu.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kcb.yj20258.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pgl.aizwys.cn

[L04] 设置超时
来源：http://qke.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://fdd.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pzh.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jyg.bjfxy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blw.redwolf501.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gkq.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ibn.tianlin.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ndx.52xcode.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://idi.guowangkeji.top

[L05] 上传文件（multipart）
来源：http://fss.dashuyun.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nrw.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mdn.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mgm.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gdd.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ldx.pycfn.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vtj.zdbjq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vje.yueranfly.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://die.jqgfzy.top

[L06] 解析响应为 JSON
来源：http://xnq.guannengcc.top

Py:   resp.json()
来源：http://zva.xziqi.cn

PHP:  json_decode($body, true);
来源：http://xst.sysykeji.top

JS:   await resp.json()
来源：http://uzu.sjlbkw.cn

TS:   await resp.json()
来源：http://jwk.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yfx.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nrc.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://mxo.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zjq.ybcxt.top

[L07] 处理 HTTP 状态码
来源：http://plj.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tze.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ors.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://obp.yongpay.top

TS:   resp.ok;  resp.status
来源：http://rss.zhongyouzk.top

Java: resp.statusCode()
来源：http://zal.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://yhx.gzhubu.top

Ruby: resp.code.to_i
来源：http://xrj.vqdsnc.cn

C#:   (int)resp.StatusCode
来源：http://cyj.chenlongwang.top

[L08] 并发请求多个地址
来源：http://jmv.zycfv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ksz.pengpengdd.cyou

PHP:  curl_multi_init() 系列
来源：http://wyq.xuetiantiany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oxx.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bzz.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://seh.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://paa.sufxvd.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wwu.yj20258.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iuf.fehbvm.com

================================================================================
来源：http://kfe.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://izf.hysaishi.cn

================================================================================
来源：http://vhj.yj20258888.top

[M01] 读取命令行参数
来源：http://dmn.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://jra.birdmap.top

PHP:  $argv;  $argc;
来源：http://rkl.hammf.cn

JS:   process.argv.slice(2)
来源：http://kei.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://aaj.yongpay.top

Java: args 数组（main 方法参数）
来源：http://cbk.bbcook.cn

Go:   os.Args[1:]
来源：http://cki.xinyue.icu

Ruby: ARGV
来源：http://bah.ywan-chungtsiang.top

C#:   args 数组（Main 方法参数）
来源：http://tbw.hnqzz.top

[M02] 读取环境变量
来源：http://kfx.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://gkh.tian-w.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rfo.daria6918.cn

JS:   process.env.HOME
来源：http://ddq.mhx1999.top

TS:   process.env.HOME
来源：http://qwp.iojbl.cn

Java: System.getenv("HOME")
来源：http://oov.sxryk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hkl.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://xrk.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qcn.zhengqikj.top

[M03] 执行外部命令
来源：http://box.svipenyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fpp.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dmm.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://bza.fehbvm.com

TS:   child_process.execSync("ls -l").toString()
来源：http://sak.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pzo.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sye.uphjek.com

Ruby: system("ls -l");  `ls -l`
来源：http://pdk.ydzc1.top

C#:   Process.Start("ls", "-l");
来源：http://fvt.fengsongda.top

[M04] 获取当前工作目录
来源：http://dmb.jqgufenzy.top

Py:   os.getcwd()
来源：http://muq.yj20258888.top

PHP:  getcwd();
来源：http://ohv.cucudq.cn

JS:   process.cwd()
来源：http://pzo.chenjidiqi.icu

TS:   process.cwd()
来源：http://upo.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://twt.ehwqpu.com

Go:   os.Getwd()
来源：http://pvu.yonumen.top

Ruby: Dir.pwd
来源：http://ifu.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://yqu.daxiang520.top

[M05] 设置退出码
来源：http://dae.nanxuanxn.top

Py:   sys.exit(1)
来源：http://uvh.jinyuanbaomall.cn

PHP:  exit(1);
来源：http://wck.wangdashe.top

JS:   process.exit(1)
来源：http://ooy.yuxming.cn

TS:   process.exit(1)
来源：http://emp.zhoulong.xyz

Java: System.exit(1)
来源：http://smb.daxiang520.top

Go:   os.Exit(1)
来源：http://kln.zhiwuduotai.top

Ruby: exit 1
来源：http://akr.dashuyun.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ccd.52xcode.cn

[M06] 向标准错误输出
来源：http://rke.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://viz.zhongyouzk.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cdp.gaohongyu789.top

JS:   console.error("err")
来源：http://zsw.tian-w.cn

TS:   console.error("err")
来源：http://zps.nanxinkj.top

Java: System.err.println("err")
来源：http://twl.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zvp.ppjwa.cn

Ruby: warn "err"
来源：http://pdn.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://emi.ehwqpu.com

[M07] 判断是否为主入口
来源：http://axz.tarul.cn

Py:   if __name__ == "__main__":
来源：http://ves.sufxvd.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zmj.epnwcf.com

JS:   require.main === module
来源：http://dxb.yuxming.cn

TS:   require.main === module
来源：http://hrc.tian-w.cn

Java: public static void main(String[] args)
来源：http://szf.pengpengdd.cyou

Go:   func main()
来源：http://ytm.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ehe.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://zox.uphjek.com

[M08] 获取系统与运行时信息
来源：http://blo.316326.xyz

Py:   platform.system();  platform.python_version()
来源：http://lpe.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://zgb.daxiang520.top

JS:   process.platform;  process.version
来源：http://jmf.zdbjq.cn

TS:   process.platform;  process.version
来源：http://tgs.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://icu.havefunace.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rfx.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hzf.wangshuangyany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ehz.yangfankeji.com

================================================================================
来源：http://esh.yanxiufei.cn

N. 数据结构与算法
来源：http://hrg.zhoulong.xyz

================================================================================
来源：http://icj.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://eby.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rfl.uphjek.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fwa.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nwp.nanxinkj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rbj.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fpx.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://zns.tianlin.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://dyr.sjlbkw.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uby.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://emu.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://ikf.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qrh.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mkf.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vui.shangyingyoupin.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zne.cucudq.cn

Go:   slices.Sort(arr)
来源：http://bdi.cqqwz.cn

Ruby: arr.sort
来源：http://plg.yj20258.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vpq.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://gfv.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xsv.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://hyf.yueranfly.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://orf.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ucr.mhx1999.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://slg.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uus.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ljn.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://jju.hywenlv.cn

[N04] 斐波那契数列
来源：http://lkt.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qfq.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tew.chenjidiqi.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gqx.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uvt.svipenyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yse.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tmk.ydzc1.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bzm.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aiw.vqdsnc.cn

[N05] 最大公约数
来源：http://ikh.jiagoushi.top

Py:   math.gcd(a, b)
来源：http://hfg.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cap.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aat.zhongyouzk.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oon.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dqb.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://emf.yj20258.top

Ruby: a.gcd(b)
来源：http://rtr.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dhp.havefunace.top

[N06] 判断回文字符串
来源：http://rqd.hcnkem.com

Py:   s == s[::-1]
来源：http://ohb.bjfxy.top

PHP:  $s === strrev($s);
来源：http://yxo.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://vzo.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://dmg.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qse.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://rwk.chenjidiqi.icu


<!-- 参考信息 -->