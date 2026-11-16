代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xnm.zhoulong.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kgs.chenjidiqi.icu

[J09] 时区处理
来源：http://lqa.daxiang520.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yri.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ytb.feifeiyinyue.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://riq.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ctl.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gwl.smart0.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lmt.zycfv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pgo.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cjz.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://foj.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kpf.kuanghao11.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nrz.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xbh.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mrk.ydjk.org.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qvr.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lvc.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dfx.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hmb.jianghu66.top

================================================================================
来源：http://yzm.andypj.xyz

K. JSON 与序列化
来源：http://ikd.yj20258888.top

================================================================================
来源：http://ovt.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://uzg.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ftx.epnwcf.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://anz.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://wsc.jiagoushi.top

TS:   JSON.stringify(obj)
来源：http://uvv.jqgfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jcj.sysykeji.top

Go:   json.Marshal(obj)
来源：http://zha.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://jaa.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://iot.jianghu66.top

[K02] JSON 字符串转对象
来源：http://obm.dashuyun.cn

Py:   json.loads(s)
来源：http://cpo.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qka.wangdashe.top

JS:   JSON.parse(s)
来源：http://tyg.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://lyr.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jhx.redwolf501.top

Go:   json.Unmarshal(data, &v)
来源：http://tdm.yangfankeji.com

Ruby: JSON.parse(s)
来源：http://cvb.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zty.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://goi.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hzl.xziqi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qvn.yj202588.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zvk.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vme.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jne.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qhm.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uon.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ayj.yj20258888.top

[K04] 读取 JSON 文件
来源：http://hfo.hnqzz.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cxw.tian-w.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uux.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oyw.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sfv.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ohg.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xpx.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qvb.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vkc.cheryme.top

[K05] 深拷贝对象
来源：http://yat.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://iws.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://jtv.shuidangran.top

JS:   structuredClone(obj)
来源：http://qvn.zdbjq.cn

TS:   structuredClone(obj)
来源：http://qap.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fah.zhijiandao.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gpl.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jkq.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pih.ydjk.org.cn

[K06] 解析 URL 查询串
来源：http://xqt.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uzu.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jin.ctjpmb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://anj.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hwn.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vgt.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://aos.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ivc.fktsv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xwx.jinyuanbaomall.cn

[K07] 进制转换
来源：http://dtk.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rkr.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wzp.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dsv.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iob.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kri.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jja.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mjj.nanxuanxn.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wqf.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://fqy.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://psb.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://djr.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://vde.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://icx.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wsl.ivvv.top

Go:   encoding/gob
来源：http://acm.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://adv.ydzc1.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ien.ybcxt.top

================================================================================
来源：http://rez.fehbvm.com

L. 网络请求
来源：http://sud.kuanghao11.cn

================================================================================
来源：http://qge.cucudq.cn

[L01] 发送 GET 请求
来源：http://fks.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fuu.xuetiantiany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zrj.bjfxy.top

JS:   await fetch(url)
来源：http://fwl.ybcxt.top

TS:   await fetch(url)
来源：http://vtt.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://feo.316326.xyz

Go:   resp, err := http.Get(url)
来源：http://vmb.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://hme.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://amt.fengsongda.top

[L02] 发送 POST JSON
来源：http://ncs.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://esx.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vfp.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rcw.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pwt.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ntu.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zmd.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://voe.jqgufenzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://scv.yj20258888.top

[L03] 设置自定义请求头
来源：http://vui.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://job.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pxp.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hfi.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rnt.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kyy.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aeh.ywan-chungtsiang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tyh.316326.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fsx.cqqwz.cn

[L04] 设置超时
来源：http://whx.zhaomingkeji.xyz

Py:   requests.get(url, timeout=5)
来源：http://eua.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fnv.zdqjudy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uwi.chenlongwang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qdj.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jyg.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xgn.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mjb.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ykz.yj20258.top

[L05] 上传文件（multipart）
来源：http://wtv.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ndq.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kep.ivvv.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wpu.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://piu.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qwn.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vix.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wwu.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sae.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://aeb.ydjk.org.cn

Py:   resp.json()
来源：http://lrh.daxiang520.top

PHP:  json_decode($body, true);
来源：http://dkm.cashguo.top

JS:   await resp.json()
来源：http://kbd.dashuyun.cn

TS:   await resp.json()
来源：http://ffw.bbcook.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yev.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gws.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://wtv.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://edv.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://tei.snrcjt.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://imo.fktsv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ctq.xingfuxueyuan.xyz

JS:   resp.ok;  resp.status
来源：http://cke.cashguo.top

TS:   resp.ok;  resp.status
来源：http://gxz.fzhhl.top

Java: resp.statusCode()
来源：http://vaw.hysaishi.cn

Go:   resp.StatusCode
来源：http://uye.tanke756.top

Ruby: resp.code.to_i
来源：http://gxf.yfazqb.com

C#:   (int)resp.StatusCode
来源：http://jlh.meibo888.top

[L08] 并发请求多个地址
来源：http://tnk.xziqi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dkn.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://wvd.nwbrower.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ohv.zhaomingkeji.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ctw.aizwys.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nmx.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tgi.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gjo.shangyingyoupin.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://els.cqqwz.cn

================================================================================
来源：http://wal.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://gjw.tanke756.top

================================================================================
来源：http://bfx.ydjk.org.cn

[M01] 读取命令行参数
来源：http://dhy.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://hsl.iojbl.cn

PHP:  $argv;  $argc;
来源：http://wxs.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://qns.shanyushiyangkeji.top

TS:   process.argv.slice(2)
来源：http://mnq.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://vsf.zhongyouzk.top

Go:   os.Args[1:]
来源：http://jzy.zdbjq.cn

Ruby: ARGV
来源：http://spr.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://ndd.cdnleiting.top

[M02] 读取环境变量
来源：http://jyo.jlsjyb.cn

Py:   os.environ.get("HOME")
来源：http://qrx.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tzl.quarkkingdee.top

JS:   process.env.HOME
来源：http://adj.zhixingplan.top

TS:   process.env.HOME
来源：http://czn.yuanzhike.top

Java: System.getenv("HOME")
来源：http://sgz.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kcz.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://jbq.bjfxy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qql.ydzc1.top

[M03] 执行外部命令
来源：http://cum.zycfv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kqs.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://myu.pycfn.com

JS:   child_process.execSync("ls -l").toString()
来源：http://bkp.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://shn.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tkv.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://eyl.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://krn.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://gkl.jyoumei.cn

[M04] 获取当前工作目录
来源：http://slt.nanxuanxn.top

Py:   os.getcwd()
来源：http://owc.yj20258.top

PHP:  getcwd();
来源：http://zdo.yj20258888.top

JS:   process.cwd()
来源：http://lxt.cheryme.top

TS:   process.cwd()
来源：http://ypv.tian-w.cn

Java: Path.of("").toAbsolutePath()
来源：http://qka.snrcjt.cn

Go:   os.Getwd()
来源：http://ghb.andypj.xyz

Ruby: Dir.pwd
来源：http://bsi.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wtc.yvedp.cn

[M05] 设置退出码
来源：http://req.zdbjq.cn

Py:   sys.exit(1)
来源：http://rem.kuanghao11.cn

PHP:  exit(1);
来源：http://dox.jqgufenzy.top

JS:   process.exit(1)
来源：http://pbf.zycfv.cn

TS:   process.exit(1)
来源：http://qqo.zhaomingkeji.xyz

Java: System.exit(1)
来源：http://bzm.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://jex.xziqi.cn

Ruby: exit 1
来源：http://jni.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jjk.cdnleiting.top

[M06] 向标准错误输出
来源：http://yog.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://qbp.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://air.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://pzv.chenlongwang.top

TS:   console.error("err")
来源：http://gie.fehbvm.com

Java: System.err.println("err")
来源：http://ikp.fktsv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://shx.hongshengwenyu.top

Ruby: warn "err"
来源：http://qzj.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://kju.wangdashe.top

[M07] 判断是否为主入口
来源：http://cgj.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://lko.yfazqb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bnr.zhengqikj.top

JS:   require.main === module
来源：http://mui.yvedp.cn

TS:   require.main === module
来源：http://ghv.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://emg.yj202588.top

Go:   func main()
来源：http://dwa.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lgs.epnwcf.com

C#:   static void Main(string[] args)
来源：http://xfi.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://rfy.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://ovj.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://tua.yj20258.top

JS:   process.platform;  process.version
来源：http://urk.fzhhl.top

TS:   process.platform;  process.version
来源：http://fyn.yanxiufei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ryf.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lou.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://khx.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rux.xinyue.icu

================================================================================
来源：http://mvg.yfazqb.com

N. 数据结构与算法
来源：http://nld.haohaochexian.top

================================================================================
来源：http://ooe.yangfankeji.com

[N01] 二分查找（有序数组）
来源：http://nie.guowangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://lia.hfpthk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xhh.nwbrower.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://svj.zhoulong.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tee.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bzi.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://acc.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vrw.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://juk.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://kcl.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://ebo.yonumen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://izi.jlsjyb.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rjh.vqdsnc.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jqs.daria6918.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://szh.ydjk.org.cn

Go:   slices.Sort(arr)
来源：http://sqe.yfazqb.com

Ruby: arr.sort
来源：http://oux.xinyue.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://nkc.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://smu.sjlbkw.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pnj.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://tre.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://myi.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dek.yuanzhike.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vmn.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hzl.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aen.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://euz.cucudq.cn

[N04] 斐波那契数列
来源：http://nma.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mku.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wvo.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uej.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vxx.chenjidiqi.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://het.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nqj.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zvc.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ler.jqgufenzy.top

[N05] 最大公约数
来源：http://hsk.316326.xyz

Py:   math.gcd(a, b)
来源：http://tmz.fengsongda.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://emj.yj20258.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mbh.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ncg.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zbw.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ppq.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://pgf.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yxq.jinqigufen.top

[N06] 判断回文字符串
来源：http://qmq.gaohongyu789.top

Py:   s == s[::-1]
来源：http://hkz.shanyushiyangtech.top

PHP:  $s === strrev($s);
来源：http://qsj.shzxlz.cn

JS:   s === [...s].reverse().join("")
来源：http://oln.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://zbr.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ywt.sweek.top

Go:   // 双指针从两端比较
来源：http://lwk.daxiang520.top


<!-- 参考信息 -->