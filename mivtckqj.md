代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gmz.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ksv.shanyushiyangkeji.top

[J09] 时区处理
来源：http://eww.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ajk.pengpengdd.cyou

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wzn.zhaomingkeji.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kcx.tanke756.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mjx.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wfc.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rwq.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sut.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nqr.mhx1999.top

[J10] 取今天 / 本月第一天
来源：http://hyx.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://als.xuetiantiany.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jee.zhixingplan.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cjj.chenlongwang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tpg.zycfv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rbe.fzhhl.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dhm.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gzk.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rmp.52xcode.cn

================================================================================
来源：http://iqr.sufxvd.cn

K. JSON 与序列化
来源：http://fqi.zhongyouzk.top

================================================================================
来源：http://hcd.cucudq.cn

[K01] 对象转 JSON 字符串
来源：http://yys.316326.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cwv.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pmu.meibo888.top

JS:   JSON.stringify(obj)
来源：http://rci.ppjwa.cn

TS:   JSON.stringify(obj)
来源：http://rht.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://avd.redwolf501.top

Go:   json.Marshal(obj)
来源：http://uag.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://nqu.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hcn.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://ftr.bbcook.cn

Py:   json.loads(s)
来源：http://aro.guowangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tqq.fanxiaobao.xyz

JS:   JSON.parse(s)
来源：http://uwm.cucudq.cn

TS:   JSON.parse(s)
来源：http://neb.andypj.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xkj.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://jfv.daria6918.cn

Ruby: JSON.parse(s)
来源：http://uka.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ckd.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://xbc.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bcp.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tfq.xuanzx.com

JS:   JSON.stringify(obj, null, 2)
来源：http://plh.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oec.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vby.andypj.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pja.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cfz.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://oow.cashguo.top

[K04] 读取 JSON 文件
来源：http://uwo.shanyushiyangtech.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gtu.xinyue.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wwf.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hku.redwolf501.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qmg.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vdb.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pja.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://zms.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://skc.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://nwq.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://eus.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://uxh.aizwys.cn

JS:   structuredClone(obj)
来源：http://dze.pengpengdd.cyou

TS:   structuredClone(obj)
来源：http://lsa.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://vla.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://otc.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ase.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://fzr.xuanzx.com

[K06] 解析 URL 查询串
来源：http://zia.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iye.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nnv.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xqi.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bjt.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://psx.zhaomingkeji.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://hzs.yj20258.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://llv.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://flj.zhijiandao.cn

[K07] 进制转换
来源：http://eul.hammf.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ivv.cucudq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mkr.sxryk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jgg.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dsi.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pex.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ibl.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wef.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aib.hysaishi.cn

[K08] 二进制序列化（非 JSON）
来源：http://yqn.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://qlz.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://mdn.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://sgs.fehbvm.com

TS:   v8.serialize(obj)        // Node
来源：http://fch.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wfe.hnxiangtu.top

Go:   encoding/gob
来源：http://wad.uphjek.com

Ruby: Marshal.dump(obj)
来源：http://ugr.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jrl.xuetiantiany.cn

================================================================================
来源：http://fjn.hysaishi.cn

L. 网络请求
来源：http://fzm.yj202588.top

================================================================================
来源：http://mfa.andypj.xyz

[L01] 发送 GET 请求
来源：http://sbk.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eft.xziqi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qnh.cheryme.top

JS:   await fetch(url)
来源：http://exm.shanyushiyangkeji.top

TS:   await fetch(url)
来源：http://pxm.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zah.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://rgk.ctjpmb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://knb.ivvv.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lkk.zhengqikj.top

[L02] 发送 POST JSON
来源：http://uzd.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://trj.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qdc.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ofd.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hls.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jvp.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tvx.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wgr.bbcook.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://grj.chenzaomai.com

[L03] 设置自定义请求头
来源：http://qbz.hnxiangtu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fkg.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uqy.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://obm.snrcjt.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zrk.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rei.sysykeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kgj.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yad.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://suh.sjlbkw.cn

[L04] 设置超时
来源：http://cyr.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://shn.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jal.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://noc.c1oappe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pih.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lgo.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oxj.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gaz.nwbrower.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vvq.fzhhl.top

[L05] 上传文件（multipart）
来源：http://enr.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tyu.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xcb.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rgj.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jfg.ppjwa.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://muy.jinghuilouyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zth.zhongyouzk.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://guk.quarkkingdee.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lgs.nwbrower.top

[L06] 解析响应为 JSON
来源：http://gse.vqdsnc.cn

Py:   resp.json()
来源：http://iwf.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://oba.cqqwz.cn

JS:   await resp.json()
来源：http://zzz.yj20258.top

TS:   await resp.json()
来源：http://irg.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://guy.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bsf.cucudq.cn

Ruby: JSON.parse(resp.body)
来源：http://yhg.yongpay.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://whw.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://hla.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://psa.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hvk.daxiang520.top

JS:   resp.ok;  resp.status
来源：http://uyi.jqgufenzy.top

TS:   resp.ok;  resp.status
来源：http://bjq.svipenyu.cn

Java: resp.statusCode()
来源：http://afu.cqqwz.cn

Go:   resp.StatusCode
来源：http://lae.0kj1m.cn

Ruby: resp.code.to_i
来源：http://loz.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://mbp.smart0.xyz

[L08] 并发请求多个地址
来源：http://yhb.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tif.jianghu66.top

PHP:  curl_multi_init() 系列
来源：http://vpm.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ljs.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jzk.zhixingplan.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vxw.fzhhl.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dpv.ywan-chungtsiang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wol.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jec.fktsv.cn

================================================================================
来源：http://cvn.bbcook.cn

M. 命令行 / 进程 / 环境
来源：http://dug.chenlongwang.top

================================================================================
来源：http://mwn.chenlongwang.top

[M01] 读取命令行参数
来源：http://vrf.birdmap.top

Py:   sys.argv[1:]
来源：http://yak.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://kwq.ywan-chungtsiang.top

JS:   process.argv.slice(2)
来源：http://kjd.wangshuangyany.cn

TS:   process.argv.slice(2)
来源：http://jwk.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://vgu.birdmap.top

Go:   os.Args[1:]
来源：http://ydw.guowangkeji.top

Ruby: ARGV
来源：http://puq.aizwys.cn

C#:   args 数组（Main 方法参数）
来源：http://wcn.redwolf501.top

[M02] 读取环境变量
来源：http://ece.fzhhl.top

Py:   os.environ.get("HOME")
来源：http://nik.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://upn.chenzaomai.com

JS:   process.env.HOME
来源：http://imc.hnqzz.top

TS:   process.env.HOME
来源：http://dur.zdbjq.cn

Java: System.getenv("HOME")
来源：http://osg.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ofc.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://wtp.zhengqikj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wzp.snrcjt.cn

[M03] 执行外部命令
来源：http://ifx.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://daf.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uhy.pycfn.com

JS:   child_process.execSync("ls -l").toString()
来源：http://kqs.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dnr.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lmt.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dox.ybcxt.top

Ruby: system("ls -l");  `ls -l`
来源：http://iug.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://cyl.tianlin.xyz

[M04] 获取当前工作目录
来源：http://zrp.jlsjyb.cn

Py:   os.getcwd()
来源：http://zet.pycfn.com

PHP:  getcwd();
来源：http://ehi.uphjek.com

JS:   process.cwd()
来源：http://zot.jiagoushi.top

TS:   process.cwd()
来源：http://bbj.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://bhy.fehbvm.com

Go:   os.Getwd()
来源：http://ovx.sweek.top

Ruby: Dir.pwd
来源：http://akc.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://ddr.jinqigufen.top

[M05] 设置退出码
来源：http://bxg.316326.xyz

Py:   sys.exit(1)
来源：http://thy.fzhhl.top

PHP:  exit(1);
来源：http://wpf.pengpengdd.cyou

JS:   process.exit(1)
来源：http://ora.gaohongyu789.top

TS:   process.exit(1)
来源：http://iul.birdmap.top

Java: System.exit(1)
来源：http://oon.yonumen.top

Go:   os.Exit(1)
来源：http://tej.fzhhl.top

Ruby: exit 1
来源：http://trh.guannengcc.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fed.cashguo.top

[M06] 向标准错误输出
来源：http://mvu.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://dwp.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ctw.hnqzz.top

JS:   console.error("err")
来源：http://hci.ybcxt.top

TS:   console.error("err")
来源：http://jqh.ydzc1.top

Java: System.err.println("err")
来源：http://sdj.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lcn.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://oyd.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://xwp.dianchejie.cn

[M07] 判断是否为主入口
来源：http://jum.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://wlh.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bhx.zhongyouzk.top

JS:   require.main === module
来源：http://pnb.hammf.cn

TS:   require.main === module
来源：http://tgn.gotoacloud.top

Java: public static void main(String[] args)
来源：http://pki.jqgfzy.top

Go:   func main()
来源：http://rue.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://awa.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://hgn.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://jpq.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://rcn.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://pzz.snrcjt.cn

JS:   process.platform;  process.version
来源：http://uei.tianlin.xyz

TS:   process.platform;  process.version
来源：http://fki.yangfankeji.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xcz.daxiang520.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rps.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cha.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://tcz.haohaochexian.top

================================================================================
来源：http://mbv.zdbjq.cn

N. 数据结构与算法
来源：http://duv.chenzaomai.com

================================================================================
来源：http://pjy.hywenlv.cn

[N01] 二分查找（有序数组）
来源：http://ata.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://xyd.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gkp.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gmq.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ewq.uphjek.com

Java: Arrays.binarySearch(arr, x)
来源：http://djn.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://gse.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://yfk.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://qnj.daxiang520.top

[N02] 排序（工程实践用内置实现）
来源：http://pqa.bbcook.cn

Py:   sorted(arr);  arr.sort()
来源：http://ojs.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bqv.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jhd.zhoulong.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://hzj.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mra.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://ppe.ppjwa.cn

Ruby: arr.sort
来源：http://sru.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gqt.bjfxy.top

[N03] 快速排序（分治示例）
来源：http://hyg.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uep.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://jme.svipenyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://afn.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://raa.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://klj.316326.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nvc.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tlu.hesvh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hko.zhiwuduotai.top

[N04] 斐波那契数列
来源：http://gig.sysykeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ret.hesvh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oeh.smart0.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cek.hywenlv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qek.ydjk.org.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kuz.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ppm.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lbi.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ffe.hnxiangtu.top

[N05] 最大公约数
来源：http://mmj.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://zqw.feifeiyinyue.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sqd.yueranfly.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fyh.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nfw.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vcl.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ywx.wangdashe.top

Ruby: a.gcd(b)
来源：http://pwq.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zpb.zycfv.cn

[N06] 判断回文字符串
来源：http://neo.sysykeji.top

Py:   s == s[::-1]
来源：http://mpe.cdnleiting.top

PHP:  $s === strrev($s);
来源：http://ttx.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://ism.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://rce.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ayh.sweek.top

Go:   // 双指针从两端比较
来源：http://cmt.jinyuanbaomall.cn


<!-- 参考信息 -->