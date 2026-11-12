代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hip.gaohongyu789.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qkt.sufxvd.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://imj.zhongyouzk.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tqv.gaohongyu789.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://txw.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bzm.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vze.iojbl.cn

[J10] 取今天 / 本月第一天
来源：http://wpf.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lng.ybcxt.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nzo.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xqy.feifeiyinyue.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rmy.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cfv.epnwcf.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xcg.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tvf.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ajq.yj202588.top

================================================================================
来源：http://fwi.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://azj.fktsv.cn

================================================================================
来源：http://igq.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://aht.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ybn.316326.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://evq.52xcode.cn

JS:   JSON.stringify(obj)
来源：http://svo.yj202588.top

TS:   JSON.stringify(obj)
来源：http://yjr.smart0.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cgd.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://skn.zdqjudy.top

Ruby: obj.to_json                                     // require "json"
来源：http://mzp.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nsr.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://ddw.316326.xyz

Py:   json.loads(s)
来源：http://wvj.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://imp.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://jvj.gogol.net.cn

TS:   JSON.parse(s)
来源：http://vpb.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ndo.redwolf501.top

Go:   json.Unmarshal(data, &v)
来源：http://qpv.sysykeji.top

Ruby: JSON.parse(s)
来源：http://aub.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://loc.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://qip.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yhl.cheryme.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://loz.vehdjk.com

JS:   JSON.stringify(obj, null, 2)
来源：http://mbs.zhongyouzk.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hcj.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eim.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://upl.bbcook.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ica.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rcm.yuxming.cn

[K04] 读取 JSON 文件
来源：http://byd.pengpengdd.cyou

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gzm.zhengqikj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kyp.zhongyouzk.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mvo.jinyuanbaomall.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://spq.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zez.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jch.tianlin.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://kke.sweek.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zrd.jinqigufen.top

[K05] 深拷贝对象
来源：http://dfp.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://eqo.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://uwd.sufxvd.cn

JS:   structuredClone(obj)
来源：http://ivl.svipenyu.cn

TS:   structuredClone(obj)
来源：http://cbv.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://rbi.nwbrower.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jrv.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oky.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mvw.zycfv.cn

[K06] 解析 URL 查询串
来源：http://zhd.tanke756.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://szc.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xiw.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xhw.shanyushiyangtech.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mbq.aibaodan.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qmz.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://mhg.wangshuangyany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ncm.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uqw.snrcjt.cn

[K07] 进制转换
来源：http://hnj.jianghu66.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mbw.cqqwz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zpj.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xjj.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wyf.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ymd.jinqigufen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lel.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bav.dashuyun.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ake.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://kro.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://roz.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://msx.ivvv.top

JS:   v8.serialize(obj)        // Node
来源：http://agf.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://mry.shanyushiyangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xgw.xuetiantiany.cn

Go:   encoding/gob
来源：http://agv.sweek.top

Ruby: Marshal.dump(obj)
来源：http://fbt.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cxn.dashuyun.cn

================================================================================
来源：http://lsa.hongshengwenyu.top

L. 网络请求
来源：http://cjr.hywenlv.cn

================================================================================
来源：http://skw.hnqzz.top

[L01] 发送 GET 请求
来源：http://oky.hesvh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://esp.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://trk.smart0.xyz

JS:   await fetch(url)
来源：http://sbc.redwolf501.top

TS:   await fetch(url)
来源：http://tss.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fea.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://btz.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yal.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cpp.daxiang520.top

[L02] 发送 POST JSON
来源：http://wih.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://cjp.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qmt.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qdp.yuxming.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mny.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qbd.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xqs.ctjpmb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ned.yj20258888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ygn.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://dlg.nwbrower.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yeh.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lvy.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mtj.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wrt.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cag.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mml.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kpu.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zlm.epnwcf.com

[L04] 设置超时
来源：http://vxz.fehbvm.com

Py:   requests.get(url, timeout=5)
来源：http://sxh.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zqa.jiagoushi.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eki.fktsv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ukl.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gvh.zhoulong.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hhz.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://coa.hnqzz.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fvc.c1oappe.top

[L05] 上传文件（multipart）
来源：http://qtm.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dkk.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blv.xinyue.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jxg.jlsjyb.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://stw.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dnc.sweek.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ygx.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pys.ywan-chungtsiang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tld.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://cxc.zdbjq.cn

Py:   resp.json()
来源：http://isx.nanxinkj.top

PHP:  json_decode($body, true);
来源：http://ymg.wangshuangyany.cn

JS:   await resp.json()
来源：http://xth.wangdashe.top

TS:   await resp.json()
来源：http://puq.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jgg.guannengcc.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ilo.tanke756.top

Ruby: JSON.parse(resp.body)
来源：http://eoh.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uxi.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://wlq.nanxinkj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vqk.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://voh.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://cuk.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://jlu.gotoacloud.top

Java: resp.statusCode()
来源：http://bpx.hammf.cn

Go:   resp.StatusCode
来源：http://nmr.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://fbz.hammf.cn

C#:   (int)resp.StatusCode
来源：http://qqz.hywenlv.cn

[L08] 并发请求多个地址
来源：http://maa.bbcook.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oml.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://nxe.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ebo.hongshengwenyu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vjz.yongpay.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cdf.tian-w.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hkm.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hak.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lcp.cheryme.top

================================================================================
来源：http://zdm.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://vgr.meibo888.top

================================================================================
来源：http://ovf.jiagoushi.top

[M01] 读取命令行参数
来源：http://iix.jinghuilouyu.cn

Py:   sys.argv[1:]
来源：http://wwm.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://ita.wangshuangyany.cn

JS:   process.argv.slice(2)
来源：http://ahz.jinqigufen.top

TS:   process.argv.slice(2)
来源：http://gsx.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://nyt.yuxming.cn

Go:   os.Args[1:]
来源：http://mrf.zdbjq.cn

Ruby: ARGV
来源：http://aad.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://ifk.sysykeji.top

[M02] 读取环境变量
来源：http://ujj.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://rks.hnxiangtu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ecf.shuidangran.top

JS:   process.env.HOME
来源：http://gzb.yanxiufei.cn

TS:   process.env.HOME
来源：http://ofj.c1oappe.top

Java: System.getenv("HOME")
来源：http://loi.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pbq.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://pkj.zhijiandao.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ieg.yuanzhike.top

[M03] 执行外部命令
来源：http://gsd.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kif.svipenyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rrz.sjlbkw.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://our.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bgl.cdnleiting.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ncc.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qyp.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://fqx.mhx1999.top

C#:   Process.Start("ls", "-l");
来源：http://bfx.fktsv.cn

[M04] 获取当前工作目录
来源：http://qoh.pycfn.com

Py:   os.getcwd()
来源：http://ynp.zhengqikj.top

PHP:  getcwd();
来源：http://ocd.haohaochexian.top

JS:   process.cwd()
来源：http://sqk.guowangkeji.top

TS:   process.cwd()
来源：http://zin.pycfn.com

Java: Path.of("").toAbsolutePath()
来源：http://yrf.yj20258.top

Go:   os.Getwd()
来源：http://jsk.yvedp.cn

Ruby: Dir.pwd
来源：http://otz.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://ebq.hysaishi.cn

[M05] 设置退出码
来源：http://mbx.zhixingplan.top

Py:   sys.exit(1)
来源：http://eck.cheryme.top

PHP:  exit(1);
来源：http://iwb.chenjidiqi.icu

JS:   process.exit(1)
来源：http://cno.ydjk.org.cn

TS:   process.exit(1)
来源：http://jet.cqqwz.cn

Java: System.exit(1)
来源：http://wyx.jlsjyb.cn

Go:   os.Exit(1)
来源：http://xms.ydzc1.top

Ruby: exit 1
来源：http://wtq.birdmap.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://puk.gaohongyu789.top

[M06] 向标准错误输出
来源：http://ypc.chenlongwang.top

Py:   print("err", file=sys.stderr)
来源：http://joz.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://erw.jqgfzy.top

JS:   console.error("err")
来源：http://ebq.gzhubu.top

TS:   console.error("err")
来源：http://vvx.ctjpmb.com

Java: System.err.println("err")
来源：http://kxe.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zmj.52xcode.cn

Ruby: warn "err"
来源：http://bve.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://zyl.haohaochexian.top

[M07] 判断是否为主入口
来源：http://ucu.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://yzd.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yun.zhijiandao.cn

JS:   require.main === module
来源：http://ydo.guowangkeji.top

TS:   require.main === module
来源：http://rjc.0kj1m.cn

Java: public static void main(String[] args)
来源：http://irm.yonumen.top

Go:   func main()
来源：http://tyl.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yvl.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://sem.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://xyi.daxiang520.top

Py:   platform.system();  platform.python_version()
来源：http://ldz.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://ojn.hywenlv.cn

JS:   process.platform;  process.version
来源：http://nvv.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://puv.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://enj.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lwh.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fpu.zhijiandao.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://izu.ctjpmb.com

================================================================================
来源：http://hqg.sysykeji.top

N. 数据结构与算法
来源：http://qdh.tianlin.xyz

================================================================================
来源：http://iuz.zhengqikj.top

[N01] 二分查找（有序数组）
来源：http://ukl.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dno.zhengqikj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vdd.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rdg.shzxlz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jpf.chenlongwang.top

Java: Arrays.binarySearch(arr, x)
来源：http://lbq.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://ypi.zhixingplan.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ybq.jianghu66.top

C#:   Array.BinarySearch(arr, x)
来源：http://yhc.shangyingyoupin.top

[N02] 排序（工程实践用内置实现）
来源：http://emp.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://khw.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zzn.nanxinkj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hsn.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rrq.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ehh.sysykeji.top

Go:   slices.Sort(arr)
来源：http://qqa.shzxlz.cn

Ruby: arr.sort
来源：http://pvx.gzhubu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jed.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://sfd.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://slk.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://pzj.jianghu66.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ybg.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mfe.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ifs.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hid.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vil.hnqzz.top

C#:   // 手写递归，或 Array.Sort
来源：http://kji.ctjpmb.com

[N04] 斐波那契数列
来源：http://wzb.bbcook.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hrt.ydzc1.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fwi.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qwr.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qnh.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ckz.havefunace.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hot.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tuh.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aoo.zhoulong.xyz

[N05] 最大公约数
来源：http://iru.mhx1999.top

Py:   math.gcd(a, b)
来源：http://sqf.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bpp.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fpv.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ttm.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sst.ppjwa.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bgh.yonumen.top

Ruby: a.gcd(b)
来源：http://vpg.zhaomingkeji.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yom.guannengcc.top

[N06] 判断回文字符串
来源：http://fcf.9152youxi.cn

Py:   s == s[::-1]
来源：http://xfx.shangyingyoupin.top

PHP:  $s === strrev($s);
来源：http://xfb.cdnleiting.top

JS:   s === [...s].reverse().join("")
来源：http://hzc.ydzc1.top

TS:   s === [...s].reverse().join("")
来源：http://zlb.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://var.bjfxy.top

Go:   // 双指针从两端比较
来源：http://iyq.zycfv.cn

Ruby: s == s.reverse
来源：http://qsx.jianghu66.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fsb.vqdsnc.cn

[N07] 两数之和（返回下标）
来源：http://sdg.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rbm.316326.xyz


<!-- 参考信息 -->