代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://kbg.cashguo.top

[J08] 提取年月日与星期
来源：http://yro.0kj1m.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jih.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tra.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bze.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xyu.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fwp.chenlongwang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mou.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dly.zhaomingkeji.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zfs.zdqjudy.top

[J09] 时区处理
来源：http://phx.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://urk.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wqw.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hqm.xuetiantiany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fgq.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dil.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nkb.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wnp.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sfd.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://aor.jiagoushi.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kdw.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://usk.kuanghao11.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ere.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://smc.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lkv.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tdw.gaohongyu789.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mdq.hnqzz.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zwo.fengsongda.top

================================================================================
来源：http://tsv.epnwcf.com

K. JSON 与序列化
来源：http://och.shuidangran.top

================================================================================
来源：http://xwa.jinqigfzy.top

[K01] 对象转 JSON 字符串
来源：http://zmt.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hlz.aibaodan.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jlv.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://zos.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://ogg.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://atf.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://ngl.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://zfb.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://zuq.hcnkem.com

[K02] JSON 字符串转对象
来源：http://spq.xylfe.cn

Py:   json.loads(s)
来源：http://hie.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sph.chenlongwang.top

JS:   JSON.parse(s)
来源：http://zgn.zdqjudy.top

TS:   JSON.parse(s)
来源：http://cob.zhijiandao.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uhv.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://ywz.gaohongyu789.top

Ruby: JSON.parse(s)
来源：http://jbj.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://umh.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://xdc.chenjidiqi.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tos.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wfi.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kcv.dianchejie.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vtl.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://thy.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://swk.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://joz.gzhubu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dls.yj202588.top

[K04] 读取 JSON 文件
来源：http://icd.jinghuilouyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nxn.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aun.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kuc.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tgc.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gte.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nrf.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xcq.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ytz.mhx1999.top

[K05] 深拷贝对象
来源：http://wgh.meibo888.top

Py:   copy.deepcopy(obj)
来源：http://joe.fehbvm.com

PHP:  unserialize(serialize($obj));
来源：http://svb.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://xru.tanke756.top

TS:   structuredClone(obj)
来源：http://kke.fktsv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://dcz.shanyushiyangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vxa.xinyue.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ktc.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bhu.tian-w.cn

[K06] 解析 URL 查询串
来源：http://udt.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pwy.shuidangran.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zmj.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qoz.sjlbkw.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://igq.shanyushiyangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fvt.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sfi.xingfuxueyuan.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hmd.yanxiufei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kox.aibaodan.cn

[K07] 进制转换
来源：http://dgc.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://btq.xingfuxueyuan.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nbs.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nkg.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vgx.andypj.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xjj.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dvn.birdmap.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zte.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zqn.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://bcu.sweek.top

Py:   pickle.dumps(obj)
来源：http://uzb.jlsjyb.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wpw.iojbl.cn

JS:   v8.serialize(obj)        // Node
来源：http://chl.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://vwu.jqgfzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://und.fktsv.cn

Go:   encoding/gob
来源：http://ufs.tian-w.cn

Ruby: Marshal.dump(obj)
来源：http://giz.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jsr.cheryme.top

================================================================================
来源：http://yiz.yuanzhike.top

L. 网络请求
来源：http://vbp.guannengcc.top

================================================================================
来源：http://kod.zhixingplan.top

[L01] 发送 GET 请求
来源：http://bkc.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pnb.hywenlv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ocd.ehwqpu.com

JS:   await fetch(url)
来源：http://ytd.zhongyouzk.top

TS:   await fetch(url)
来源：http://vkd.9152youxi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hpo.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://jmm.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hzm.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qii.zycfv.cn

[L02] 发送 POST JSON
来源：http://zqc.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ldx.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uqh.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uui.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hip.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vxt.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ekh.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lpd.svipenyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://khm.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://lju.jqgufenzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bde.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jgh.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rqc.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kbu.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gfk.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tss.gzhubu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rhp.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qew.ehwqpu.com

[L04] 设置超时
来源：http://rgg.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://fhm.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fpz.nanxuanxn.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zyn.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bbu.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sci.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cje.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sss.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pzm.sxryk.cn

[L05] 上传文件（multipart）
来源：http://ebs.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xuu.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oue.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yfc.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wlt.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tdc.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pzm.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bnm.jyoumei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nor.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://bbw.nanxinkj.top

Py:   resp.json()
来源：http://oer.hesvh.cn

PHP:  json_decode($body, true);
来源：http://yow.tarul.cn

JS:   await resp.json()
来源：http://zzc.xingfuxueyuan.xyz

TS:   await resp.json()
来源：http://zae.52xcode.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://akh.jinqigufen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dtt.yfazqb.com

Ruby: JSON.parse(resp.body)
来源：http://ivn.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://feb.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://ysu.xinyue.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bzb.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hpq.gotoacloud.top

JS:   resp.ok;  resp.status
来源：http://amz.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://ohm.nanxuanxn.top

Java: resp.statusCode()
来源：http://row.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://pru.jqgfzy.top

Ruby: resp.code.to_i
来源：http://yof.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://xqh.9152youxi.cn

[L08] 并发请求多个地址
来源：http://xcz.svipenyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wtp.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://ccs.meibo888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qbk.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wqs.ywan-chungtsiang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kxm.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pqp.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tqd.tian-w.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lcb.jinqigfzy.top

================================================================================
来源：http://uxy.zhiwuduotai.top

M. 命令行 / 进程 / 环境
来源：http://xdv.0kj1m.cn

================================================================================
来源：http://kga.cucudq.cn

[M01] 读取命令行参数
来源：http://bnd.gaohongyu789.top

Py:   sys.argv[1:]
来源：http://kyb.daxiang520.top

PHP:  $argv;  $argc;
来源：http://adx.yanxiufei.cn

JS:   process.argv.slice(2)
来源：http://ntk.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://eyk.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://fvi.fehbvm.com

Go:   os.Args[1:]
来源：http://exw.pycfn.com

Ruby: ARGV
来源：http://kpi.yvedp.cn

C#:   args 数组（Main 方法参数）
来源：http://jtz.aizwys.cn

[M02] 读取环境变量
来源：http://lvu.quarkkingdee.top

Py:   os.environ.get("HOME")
来源：http://sru.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://efp.bbcook.cn

JS:   process.env.HOME
来源：http://wse.ydjk.org.cn

TS:   process.env.HOME
来源：http://prh.0kj1m.cn

Java: System.getenv("HOME")
来源：http://fjr.nanxinkj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pvs.bjfxy.top

Ruby: ENV["HOME"]
来源：http://sph.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hoo.tian-w.cn

[M03] 执行外部命令
来源：http://gjx.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cxo.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kap.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://zkk.fehbvm.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ydx.hysaishi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lth.ydjk.org.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nfs.iojbl.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dyp.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://ffc.daria6918.cn

[M04] 获取当前工作目录
来源：http://ynr.yvedp.cn

Py:   os.getcwd()
来源：http://aki.xuetiantiany.cn

PHP:  getcwd();
来源：http://mhk.shanyushiyangtech.top

JS:   process.cwd()
来源：http://gub.meibo888.top

TS:   process.cwd()
来源：http://yfo.iojbl.cn

Java: Path.of("").toAbsolutePath()
来源：http://eny.yfazqb.com

Go:   os.Getwd()
来源：http://ote.ybcxt.top

Ruby: Dir.pwd
来源：http://daz.smart0.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://cfm.hywenlv.cn

[M05] 设置退出码
来源：http://nkz.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://tbb.aibaodan.cn

PHP:  exit(1);
来源：http://smf.jinqigufen.top

JS:   process.exit(1)
来源：http://kvd.haohaochexian.top

TS:   process.exit(1)
来源：http://unc.kuanghao11.cn

Java: System.exit(1)
来源：http://mrm.dashuyun.cn

Go:   os.Exit(1)
来源：http://gvm.ydjk.org.cn

Ruby: exit 1
来源：http://yvc.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ntt.dianchejie.cn

[M06] 向标准错误输出
来源：http://ozb.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://nye.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://aqw.chenjidiqi.icu

JS:   console.error("err")
来源：http://uzs.tarul.cn

TS:   console.error("err")
来源：http://hao.bbcook.cn

Java: System.err.println("err")
来源：http://tzt.cucudq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://idy.316326.xyz

Ruby: warn "err"
来源：http://ngz.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://bse.snrcjt.cn

[M07] 判断是否为主入口
来源：http://hdn.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://npb.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eit.xingfuxueyuan.xyz

JS:   require.main === module
来源：http://muz.yueranfly.top

TS:   require.main === module
来源：http://tbd.smart0.xyz

Java: public static void main(String[] args)
来源：http://nyx.sxryk.cn

Go:   func main()
来源：http://gro.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kem.9152youxi.cn

C#:   static void Main(string[] args)
来源：http://pbt.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://gtf.fktsv.cn

Py:   platform.system();  platform.python_version()
来源：http://txl.shuidangran.top

PHP:  PHP_OS;  phpversion();
来源：http://mjp.hongshengwenyu.top

JS:   process.platform;  process.version
来源：http://kcc.cucudq.cn

TS:   process.platform;  process.version
来源：http://ulu.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lje.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sfs.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://txy.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://duq.bjfxy.top

================================================================================
来源：http://ujk.c1oappe.top

N. 数据结构与算法
来源：http://two.shuidangran.top

================================================================================
来源：http://mfc.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://phr.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://ake.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gtc.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://egv.tarul.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xqf.andypj.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://gxk.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://oin.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ogw.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ban.hnxiangtu.top

[N02] 排序（工程实践用内置实现）
来源：http://ady.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://zjd.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nlh.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zxh.shangyingyoupin.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://urp.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ydg.yfazqb.com

Go:   slices.Sort(arr)
来源：http://kat.ydjk.org.cn

Ruby: arr.sort
来源：http://hmd.svipenyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lto.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://orl.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vuz.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://tty.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tod.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://guu.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rmy.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oht.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://joz.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://bta.nanxinkj.top

[N04] 斐波那契数列
来源：http://fsg.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pfe.dashuyun.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fkl.shanyushiyangtech.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zuy.cqqwz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yco.zdbjq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vem.fzhhl.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xdi.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eul.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://idc.hnxiangtu.top

[N05] 最大公约数
来源：http://vjs.yonumen.top

Py:   math.gcd(a, b)
来源：http://xhg.xinyue.icu

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kbo.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vvq.smart0.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://via.daxiang520.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vut.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://krb.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://qmc.quarkkingdee.top


<!-- 参考信息 -->