代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://gwp.ybcxt.top

[J08] 提取年月日与星期
来源：http://rjw.zhijiandao.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ifc.yj20258.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cuj.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oow.ydjk.org.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lma.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rgv.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ubj.cucudq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vut.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tjk.xuetiantiany.cn

[J09] 时区处理
来源：http://eaw.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ypd.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://luy.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rkm.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ult.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gxb.fktsv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xuw.shangyingyoupin.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ijr.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ejv.yongpay.top

[J10] 取今天 / 本月第一天
来源：http://glg.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xyu.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aeg.yj20258.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dpx.zhengqikj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cvi.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://acg.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ewf.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xih.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lvn.xuetiantiany.cn

================================================================================
来源：http://gmn.chenzaomai.com

K. JSON 与序列化
来源：http://stp.fehbvm.com

================================================================================
来源：http://rip.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://rcm.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hkz.fktsv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iqk.sxryk.cn

JS:   JSON.stringify(obj)
来源：http://svy.cucudq.cn

TS:   JSON.stringify(obj)
来源：http://ltm.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://knt.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://pjf.guowangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://lim.shuidangran.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ehr.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://mcl.xinyue.icu

Py:   json.loads(s)
来源：http://yvh.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jyx.xylfe.cn

JS:   JSON.parse(s)
来源：http://fxn.dashuyun.cn

TS:   JSON.parse(s)
来源：http://yxx.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fxe.zhijiandao.cn

Go:   json.Unmarshal(data, &v)
来源：http://mza.havefunace.top

Ruby: JSON.parse(s)
来源：http://vva.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ucd.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://otu.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vvm.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pva.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yif.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://yxp.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fbt.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nby.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://xnr.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://plr.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://nqm.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://acg.ctjpmb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yol.bjfxy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gvg.zhoulong.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jdg.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pti.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uxq.zhoulong.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://efo.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zua.zhongyouzk.top

[K05] 深拷贝对象
来源：http://guu.zhoulong.xyz

Py:   copy.deepcopy(obj)
来源：http://ttt.9152youxi.cn

PHP:  unserialize(serialize($obj));
来源：http://dnj.xingfuxueyuan.xyz

JS:   structuredClone(obj)
来源：http://tjs.cucudq.cn

TS:   structuredClone(obj)
来源：http://fbu.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ovq.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lxu.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lrs.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://kod.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://bwk.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://onz.epnwcf.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nqz.nwbrower.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ifd.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qag.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hca.zycfv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tih.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wwe.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://epx.xziqi.cn

[K07] 进制转换
来源：http://ekz.bbcook.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wod.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://euh.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vrt.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hxz.chenzaomai.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vpk.dashuyun.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hla.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qdn.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nxc.ivvv.top

[K08] 二进制序列化（非 JSON）
来源：http://osr.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://rvd.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zyp.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://lqj.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://dir.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lvy.sufxvd.cn

Go:   encoding/gob
来源：http://hbv.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://huv.wangshuangyany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://smd.jinqigufen.top

================================================================================
来源：http://fww.daxiang520.top

L. 网络请求
来源：http://mfa.sysykeji.top

================================================================================
来源：http://nbs.zhixingplan.top

[L01] 发送 GET 请求
来源：http://uua.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hlu.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dvj.zhijiandao.cn

JS:   await fetch(url)
来源：http://rkr.cqqwz.cn

TS:   await fetch(url)
来源：http://jov.zhijiandao.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aha.shzxlz.cn

Go:   resp, err := http.Get(url)
来源：http://ppa.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vgm.sufxvd.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jky.gotoacloud.top

[L02] 发送 POST JSON
来源：http://vyt.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://tpi.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eda.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jio.sxryk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xlg.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://njq.daxiang520.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ahn.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bbl.yvedp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fdy.0kj1m.cn

[L03] 设置自定义请求头
来源：http://bgt.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://clx.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bii.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mbe.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wkf.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://idq.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ydp.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ohl.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fiw.yvedp.cn

[L04] 设置超时
来源：http://muw.gogol.net.cn

Py:   requests.get(url, timeout=5)
来源：http://fwr.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pdb.cashguo.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eqi.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qvs.redwolf501.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nvi.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bdq.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wsw.jyoumei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lad.shanyushiyangkeji.top

[L05] 上传文件（multipart）
来源：http://pdi.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dlg.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tbg.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aqc.shzxlz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wdq.gogol.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vqq.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jnv.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kvx.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lts.daria6918.cn

[L06] 解析响应为 JSON
来源：http://prc.sufxvd.cn

Py:   resp.json()
来源：http://fkk.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://lod.jianghu66.top

JS:   await resp.json()
来源：http://mxl.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://bai.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://esb.yj20258888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fmt.shuidangran.top

Ruby: JSON.parse(resp.body)
来源：http://hdk.chenlongwang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qtc.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://suo.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wey.xinyue.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ygf.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://rdp.iojbl.cn

TS:   resp.ok;  resp.status
来源：http://sjm.ivvv.top

Java: resp.statusCode()
来源：http://hzo.ybcxt.top

Go:   resp.StatusCode
来源：http://vds.tarul.cn

Ruby: resp.code.to_i
来源：http://twz.andypj.xyz

C#:   (int)resp.StatusCode
来源：http://hhp.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://wab.hongshengwenyu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vxj.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://fjl.zhaomingkeji.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://epq.hywenlv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://efb.316326.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gxc.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zic.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://meh.sysykeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tur.zhongyouzk.top

================================================================================
来源：http://yad.ydjk.org.cn

M. 命令行 / 进程 / 环境
来源：http://vtp.52xcode.cn

================================================================================
来源：http://mne.shzxlz.cn

[M01] 读取命令行参数
来源：http://cjv.jinqigfzy.top

Py:   sys.argv[1:]
来源：http://sjv.smart0.xyz

PHP:  $argv;  $argc;
来源：http://sve.chenjidiqi.icu

JS:   process.argv.slice(2)
来源：http://uek.jqgfzy.top

TS:   process.argv.slice(2)
来源：http://ncx.zhixingplan.top

Java: args 数组（main 方法参数）
来源：http://qeh.aizwys.cn

Go:   os.Args[1:]
来源：http://ieg.tian-w.cn

Ruby: ARGV
来源：http://kpb.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://uxd.yj20258.top

[M02] 读取环境变量
来源：http://lps.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://dcz.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://anm.cucudq.cn

JS:   process.env.HOME
来源：http://lpa.jqgfzy.top

TS:   process.env.HOME
来源：http://dso.bbcook.cn

Java: System.getenv("HOME")
来源：http://lhk.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ntw.yj202588.top

Ruby: ENV["HOME"]
来源：http://lre.fehbvm.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fqh.zdbjq.cn

[M03] 执行外部命令
来源：http://oce.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://erq.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://inn.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://mlr.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qwa.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cfu.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://akp.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://fji.yuanzhike.top

C#:   Process.Start("ls", "-l");
来源：http://gxu.ehwqpu.com

[M04] 获取当前工作目录
来源：http://ycc.quarkkingdee.top

Py:   os.getcwd()
来源：http://rhy.hfpthk.cn

PHP:  getcwd();
来源：http://hnx.daxiang520.top

JS:   process.cwd()
来源：http://qee.hongshengwenyu.top

TS:   process.cwd()
来源：http://scs.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://hhu.dashuyun.cn

Go:   os.Getwd()
来源：http://vmk.nwbrower.top

Ruby: Dir.pwd
来源：http://hir.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lae.haohaochexian.top

[M05] 设置退出码
来源：http://ljw.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://ofe.yonumen.top

PHP:  exit(1);
来源：http://gwi.hysaishi.cn

JS:   process.exit(1)
来源：http://xew.hnxiangtu.top

TS:   process.exit(1)
来源：http://jlb.gogol.net.cn

Java: System.exit(1)
来源：http://moh.tian-w.cn

Go:   os.Exit(1)
来源：http://nya.zycfv.cn

Ruby: exit 1
来源：http://rty.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yxq.cheryme.top

[M06] 向标准错误输出
来源：http://git.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://wyw.pengpengdd.cyou

PHP:  fwrite(STDERR, "err\n");
来源：http://ulr.yonumen.top

JS:   console.error("err")
来源：http://jhq.bbcook.cn

TS:   console.error("err")
来源：http://rof.ctjpmb.com

Java: System.err.println("err")
来源：http://aal.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://raj.zdbjq.cn

Ruby: warn "err"
来源：http://otc.jiagoushi.top

C#:   Console.Error.WriteLine("err")
来源：http://vfs.bbcook.cn

[M07] 判断是否为主入口
来源：http://ymk.tarul.cn

Py:   if __name__ == "__main__":
来源：http://shf.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zhq.feifeiyinyue.top

JS:   require.main === module
来源：http://ycq.ehwqpu.com

TS:   require.main === module
来源：http://rnr.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://gqz.fehbvm.com

Go:   func main()
来源：http://uzr.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xxy.havefunace.top

C#:   static void Main(string[] args)
来源：http://mws.yj202588.top

[M08] 获取系统与运行时信息
来源：http://pso.ywan-chungtsiang.top

Py:   platform.system();  platform.python_version()
来源：http://mmt.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://uih.316326.xyz

JS:   process.platform;  process.version
来源：http://vym.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://whd.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://abz.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://iti.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jmo.yj20258.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://aon.zhoulong.xyz

================================================================================
来源：http://opv.fktsv.cn

N. 数据结构与算法
来源：http://zsm.shanyushiyangtech.top

================================================================================
来源：http://jwe.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://gob.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://zii.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qwj.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fif.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://djm.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://teb.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://doz.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://utq.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://dlu.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://lha.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://ckj.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ugi.fzhhl.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://czh.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tru.fanxiaobao.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eaw.xziqi.cn

Go:   slices.Sort(arr)
来源：http://aug.jinqigufen.top

Ruby: arr.sort
来源：http://ave.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://mdd.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://rhr.dianchejie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://shr.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://oql.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fwf.xziqi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://grs.shangyingyoupin.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iuj.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://app.birdmap.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uha.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://awe.hfpthk.cn

[N04] 斐波那契数列
来源：http://nwy.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nfj.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hng.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uhr.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wro.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://inc.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://noi.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dab.dashuyun.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://knb.daxiang520.top

[N05] 最大公约数
来源：http://toi.sufxvd.cn

Py:   math.gcd(a, b)
来源：http://eda.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vua.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ohx.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cgx.pycfn.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://niy.ydjk.org.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fzl.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://ika.chenlongwang.top


<!-- 参考信息 -->