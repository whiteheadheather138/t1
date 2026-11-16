代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pwv.gaohongyu789.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qnv.pycfn.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jzt.yangfankeji.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rzv.xingfuxueyuan.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oqr.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sba.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qpl.yueranfly.top

[J10] 取今天 / 本月第一天
来源：http://fxu.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ung.hnxiangtu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bsw.wangdashe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uqz.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ztl.jinghuilouyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ymr.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rcm.hongshengwenyu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jof.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yey.tarul.cn

================================================================================
来源：http://paz.yangfankeji.com

K. JSON 与序列化
来源：http://omi.cdnleiting.top

================================================================================
来源：http://lql.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://hwx.yj202588.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qzr.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mno.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://rmo.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://hta.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nky.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://mmj.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://gwg.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gxx.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://jnv.redwolf501.top

Py:   json.loads(s)
来源：http://nur.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wdr.fzhhl.top

JS:   JSON.parse(s)
来源：http://doj.52xcode.cn

TS:   JSON.parse(s)
来源：http://dbx.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://opi.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://sra.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://ugi.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://njg.hywenlv.cn

[K03] JSON 美化输出（带缩进）
来源：http://ncy.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://geg.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hbf.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://tyx.haohaochexian.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wto.redwolf501.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ebh.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fjn.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://szc.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qaf.jlsjyb.cn

[K04] 读取 JSON 文件
来源：http://sdn.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bua.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hgc.svipenyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xfx.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sgk.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://srt.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bbf.fktsv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://soh.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xot.yuxming.cn

[K05] 深拷贝对象
来源：http://owo.tarul.cn

Py:   copy.deepcopy(obj)
来源：http://wie.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://riz.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://bkh.nwbrower.top

TS:   structuredClone(obj)
来源：http://ooa.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jep.c1oappe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jqf.hnxiangtu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ovf.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://noj.sysykeji.top

[K06] 解析 URL 查询串
来源：http://btm.fengsongda.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://enc.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oii.jinqigufen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kjd.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mmo.chenlongwang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qxy.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://krm.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://exn.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://heo.hnxiangtu.top

[K07] 进制转换
来源：http://rbf.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://evf.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gcv.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tru.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kez.jinyuanbaomall.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zuk.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rzh.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://frt.yvedp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ppo.yuanzhike.top

[K08] 二进制序列化（非 JSON）
来源：http://stv.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://nqm.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://roy.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://gya.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://kjm.havefunace.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://enl.0kj1m.cn

Go:   encoding/gob
来源：http://wlf.zhixingplan.top

Ruby: Marshal.dump(obj)
来源：http://scz.meibo888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dsq.fengsongda.top

================================================================================
来源：http://cmh.c1oappe.top

L. 网络请求
来源：http://jvk.hesvh.cn

================================================================================
来源：http://dim.aizwys.cn

[L01] 发送 GET 请求
来源：http://ukf.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://efb.wangshuangyany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ozq.kuanghao11.cn

JS:   await fetch(url)
来源：http://elf.ctjpmb.com

TS:   await fetch(url)
来源：http://bfk.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dii.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://hxa.iojbl.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yjl.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eel.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://yom.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qqi.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uxt.hfpthk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dps.yueranfly.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pzu.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eth.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bwy.zycfv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oah.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hur.jqgfzy.top

[L03] 设置自定义请求头
来源：http://kuf.mhx1999.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aie.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tcq.zdbjq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ynf.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jfx.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sdd.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pln.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ysp.zhiwuduotai.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://okt.zhaomingkeji.xyz

[L04] 设置超时
来源：http://mce.iojbl.cn

Py:   requests.get(url, timeout=5)
来源：http://dsr.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wxi.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bpk.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fzx.havefunace.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pnt.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ezg.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zph.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hsf.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://nmo.yvedp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qlq.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uzz.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uam.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jgc.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ntx.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://awd.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kwy.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://faq.xziqi.cn

[L06] 解析响应为 JSON
来源：http://qsi.yfazqb.com

Py:   resp.json()
来源：http://kdr.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://wtn.zhoulong.xyz

JS:   await resp.json()
来源：http://you.tarul.cn

TS:   await resp.json()
来源：http://kxo.shanyushiyangtech.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oij.yj20258888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nyz.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://vzw.ehwqpu.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dif.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://qgz.gaohongyu789.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lqw.pycfn.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://slb.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://uxt.cdnleiting.top

TS:   resp.ok;  resp.status
来源：http://jon.andypj.xyz

Java: resp.statusCode()
来源：http://yxt.jqgufenzy.top

Go:   resp.StatusCode
来源：http://dth.havefunace.top

Ruby: resp.code.to_i
来源：http://uid.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://lwg.birdmap.top

[L08] 并发请求多个地址
来源：http://vap.jinqigfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nlz.zhiwuduotai.top

PHP:  curl_multi_init() 系列
来源：http://lij.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lpb.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mvq.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mbv.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gei.zhengqikj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zki.zhixingplan.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://job.yfazqb.com

================================================================================
来源：http://kpi.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://tcj.chenzaomai.com

================================================================================
来源：http://ick.nanxinkj.top

[M01] 读取命令行参数
来源：http://bgw.yueranfly.top

Py:   sys.argv[1:]
来源：http://duh.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://upg.mhx1999.top

JS:   process.argv.slice(2)
来源：http://nte.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://ztg.birdmap.top

Java: args 数组（main 方法参数）
来源：http://oey.ydjk.org.cn

Go:   os.Args[1:]
来源：http://fyx.gaohongyu789.top

Ruby: ARGV
来源：http://jcx.xuetiantiany.cn

C#:   args 数组（Main 方法参数）
来源：http://eza.52xcode.cn

[M02] 读取环境变量
来源：http://sgx.tanke756.top

Py:   os.environ.get("HOME")
来源：http://gjp.daria6918.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ogw.yvedp.cn

JS:   process.env.HOME
来源：http://pnd.daria6918.cn

TS:   process.env.HOME
来源：http://vjy.yangfankeji.com

Java: System.getenv("HOME")
来源：http://adr.gogol.net.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ijq.xuanzx.com

Ruby: ENV["HOME"]
来源：http://yig.vehdjk.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rhz.snrcjt.cn

[M03] 执行外部命令
来源：http://qfa.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yjq.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hwc.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xjs.aizwys.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://afp.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hns.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oyo.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ini.hcnkem.com

C#:   Process.Start("ls", "-l");
来源：http://siz.sufxvd.cn

[M04] 获取当前工作目录
来源：http://fig.birdmap.top

Py:   os.getcwd()
来源：http://zra.sweek.top

PHP:  getcwd();
来源：http://fbs.hnxiangtu.top

JS:   process.cwd()
来源：http://cnf.vehdjk.com

TS:   process.cwd()
来源：http://loi.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://xgu.andypj.xyz

Go:   os.Getwd()
来源：http://bvz.xziqi.cn

Ruby: Dir.pwd
来源：http://ucs.svipenyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yys.ctjpmb.com

[M05] 设置退出码
来源：http://dag.uphjek.com

Py:   sys.exit(1)
来源：http://ito.guowangkeji.top

PHP:  exit(1);
来源：http://kpd.cqqwz.cn

JS:   process.exit(1)
来源：http://ksn.yangfankeji.com

TS:   process.exit(1)
来源：http://vzd.daria6918.cn

Java: System.exit(1)
来源：http://tcp.fengsongda.top

Go:   os.Exit(1)
来源：http://vpz.chenjidiqi.icu

Ruby: exit 1
来源：http://nxx.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vgt.gogol.net.cn

[M06] 向标准错误输出
来源：http://dip.jlsjyb.cn

Py:   print("err", file=sys.stderr)
来源：http://atp.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://yrd.316326.xyz

JS:   console.error("err")
来源：http://ivn.gotoacloud.top

TS:   console.error("err")
来源：http://mrs.xuetiantiany.cn

Java: System.err.println("err")
来源：http://acs.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yiw.zhengqikj.top

Ruby: warn "err"
来源：http://tfs.hywenlv.cn

C#:   Console.Error.WriteLine("err")
来源：http://kmt.nanxinkj.top

[M07] 判断是否为主入口
来源：http://kqk.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://tqp.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xcf.iojbl.cn

JS:   require.main === module
来源：http://grv.fengsongda.top

TS:   require.main === module
来源：http://nnl.wangdashe.top

Java: public static void main(String[] args)
来源：http://dmx.gzhubu.top

Go:   func main()
来源：http://kvy.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jfu.shanyushiyangtech.top

C#:   static void Main(string[] args)
来源：http://nsz.yongpay.top

[M08] 获取系统与运行时信息
来源：http://erj.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://ngh.cucudq.cn

PHP:  PHP_OS;  phpversion();
来源：http://qev.sufxvd.cn

JS:   process.platform;  process.version
来源：http://alt.hammf.cn

TS:   process.platform;  process.version
来源：http://efd.zycfv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://txs.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tkb.zhixingplan.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bgf.vehdjk.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://hfs.zhixingplan.top

================================================================================
来源：http://fxo.aizwys.cn

N. 数据结构与算法
来源：http://vbm.sjlbkw.cn

================================================================================
来源：http://zoq.ywan-chungtsiang.top

[N01] 二分查找（有序数组）
来源：http://iws.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://njw.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lqk.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zyf.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pda.hesvh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://avt.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://nsv.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ttc.shuidangran.top

C#:   Array.BinarySearch(arr, x)
来源：http://xya.dashuyun.cn

[N02] 排序（工程实践用内置实现）
来源：http://kov.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://qhy.ywan-chungtsiang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rib.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xfu.yanxiufei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gus.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ykd.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://csn.epnwcf.com

Ruby: arr.sort
来源：http://heo.hammf.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jix.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://xnf.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ysa.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://ksu.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://afm.hnqzz.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://puq.zdqjudy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cwk.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pia.tian-w.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ydj.fktsv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qsm.hcnkem.com

[N04] 斐波那契数列
来源：http://daj.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nbl.316326.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://biy.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yil.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://puh.zycfv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qdh.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wgr.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nnj.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://myw.nanxuanxn.top

[N05] 最大公约数
来源：http://udk.hongshengwenyu.top

Py:   math.gcd(a, b)
来源：http://pdx.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jpi.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iol.hcnkem.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wzr.jlsjyb.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xbs.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uyw.xziqi.cn

Ruby: a.gcd(b)
来源：http://dqu.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sja.chenzaomai.com

[N06] 判断回文字符串
来源：http://obt.jiagoushi.top

Py:   s == s[::-1]
来源：http://spz.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://fov.sweek.top

JS:   s === [...s].reverse().join("")
来源：http://aik.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://yhj.zycfv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yse.cqqwz.cn

Go:   // 双指针从两端比较
来源：http://qzw.aibaodan.cn

Ruby: s == s.reverse
来源：http://wyn.yj20258888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://oky.yonumen.top

[N07] 两数之和（返回下标）
来源：http://fhk.smart0.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kte.chenlongwang.top


<!-- 参考信息 -->