代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://aig.zhengqikj.top

[J08] 提取年月日与星期
来源：http://wsu.yuanzhike.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tuf.jiagoushi.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ftm.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://swq.xziqi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lek.jiagoushi.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://icn.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rdb.shangyingyoupin.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zid.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yoi.tarul.cn

[J09] 时区处理
来源：http://zzl.52xcode.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jrd.daxiang520.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ohb.gotoacloud.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hbf.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ebr.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zhq.hcnkem.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kxe.shanyushiyangtech.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lgt.jinqigufen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jnq.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://uba.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://imc.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mbw.ywan-chungtsiang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vkx.tian-w.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nsy.tian-w.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uxl.nanxuanxn.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dys.aizwys.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vwv.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vvy.xziqi.cn

================================================================================
来源：http://aux.yuanzhike.top

K. JSON 与序列化
来源：http://maq.hnxiangtu.top

================================================================================
来源：http://eon.vehdjk.com

[K01] 对象转 JSON 字符串
来源：http://blp.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xhd.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sar.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://yoa.sysykeji.top

TS:   JSON.stringify(obj)
来源：http://cdv.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://geb.hesvh.cn

Go:   json.Marshal(obj)
来源：http://bak.jqgufenzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://igb.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ayb.sxryk.cn

[K02] JSON 字符串转对象
来源：http://ovo.uphjek.com

Py:   json.loads(s)
来源：http://iqh.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vov.shuidangran.top

JS:   JSON.parse(s)
来源：http://wxm.daxiang520.top

TS:   JSON.parse(s)
来源：http://qyy.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qgr.xinyue.icu

Go:   json.Unmarshal(data, &v)
来源：http://yud.quarkkingdee.top

Ruby: JSON.parse(s)
来源：http://yzb.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bie.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://npq.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cjm.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qxz.birdmap.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cft.cucudq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nty.daxiang520.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://doy.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eqq.sufxvd.cn

Ruby: JSON.pretty_generate(obj)
来源：http://msp.fehbvm.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nab.yongpay.top

[K04] 读取 JSON 文件
来源：http://ipi.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ihq.jlsjyb.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bpm.zhaomingkeji.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://drz.svipenyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mto.hammf.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lrz.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yfv.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tfk.hammf.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vxp.hesvh.cn

[K05] 深拷贝对象
来源：http://gno.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://qwq.yongpay.top

PHP:  unserialize(serialize($obj));
来源：http://cdy.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://acm.fktsv.cn

TS:   structuredClone(obj)
来源：http://xcu.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tig.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://avb.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hxk.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://odc.andypj.xyz

[K06] 解析 URL 查询串
来源：http://dou.jinqigfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dyy.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xty.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rdi.aibaodan.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://udt.shanyushiyangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://arr.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cas.0kj1m.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ujk.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rdo.shanyushiyangkeji.top

[K07] 进制转换
来源：http://xkl.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nsi.birdmap.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kmc.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://enp.fengsongda.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hig.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://htt.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://npl.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sew.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hmw.zhongyouzk.top

[K08] 二进制序列化（非 JSON）
来源：http://jrp.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://wim.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://hmf.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://paw.redwolf501.top

TS:   v8.serialize(obj)        // Node
来源：http://bpn.daria6918.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://smu.vehdjk.com

Go:   encoding/gob
来源：http://abk.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://uju.shuidangran.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://stc.52xcode.cn

================================================================================
来源：http://cwo.nwbrower.top

L. 网络请求
来源：http://tte.fehbvm.com

================================================================================
来源：http://agp.daria6918.cn

[L01] 发送 GET 请求
来源：http://yrt.yonumen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://phj.gzhubu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lxh.nwbrower.top

JS:   await fetch(url)
来源：http://ehf.yongpay.top

TS:   await fetch(url)
来源：http://qgc.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hnq.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://olc.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ynm.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rfn.haohaochexian.top

[L02] 发送 POST JSON
来源：http://xbf.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://etx.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cxe.cucudq.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lze.hesvh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ahe.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xlp.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ewg.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kqj.jqgfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sed.52xcode.cn

[L03] 设置自定义请求头
来源：http://unx.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dnq.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ayy.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://awh.snrcjt.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mpq.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lay.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bhm.zhijiandao.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://irb.shanyushiyangtech.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zgs.yonumen.top

[L04] 设置超时
来源：http://sil.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://wzj.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lxy.ivvv.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ppf.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zrp.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ohw.jyoumei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fji.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rmf.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zcc.iojbl.cn

[L05] 上传文件（multipart）
来源：http://mjv.jlsjyb.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wkn.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wue.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://plu.9152youxi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ocp.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hus.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gse.shzxlz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hxw.xziqi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://izc.0kj1m.cn

[L06] 解析响应为 JSON
来源：http://ond.jianghu66.top

Py:   resp.json()
来源：http://kcc.xinyue.icu

PHP:  json_decode($body, true);
来源：http://isg.yanxiufei.cn

JS:   await resp.json()
来源：http://xgj.havefunace.top

TS:   await resp.json()
来源：http://ved.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hal.sjlbkw.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jia.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://muu.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fanxiaobao.xyz

[L07] 处理 HTTP 状态码
来源：http://tjn.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xpv.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://enh.jinqigfzy.top

JS:   resp.ok;  resp.status
来源：http://igp.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://ocs.feifeiyinyue.top

Java: resp.statusCode()
来源：http://pdx.hnxiangtu.top

Go:   resp.StatusCode
来源：http://wfj.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://wru.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://sgg.mhx1999.top

[L08] 并发请求多个地址
来源：http://cja.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tmi.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://slf.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hns.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zau.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ebo.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://adi.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qul.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gyf.quarkkingdee.top

================================================================================
来源：http://udg.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://iuh.zycfv.cn

================================================================================
来源：http://wmh.svipenyu.cn

[M01] 读取命令行参数
来源：http://kyq.guannengcc.top

Py:   sys.argv[1:]
来源：http://jgg.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://hrr.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://ohz.vehdjk.com

TS:   process.argv.slice(2)
来源：http://qib.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://dwj.ppjwa.cn

Go:   os.Args[1:]
来源：http://tdi.jlsjyb.cn

Ruby: ARGV
来源：http://wzs.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://nqc.meibo888.top

[M02] 读取环境变量
来源：http://oik.havefunace.top

Py:   os.environ.get("HOME")
来源：http://mnv.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lou.wangdashe.top

JS:   process.env.HOME
来源：http://zxr.sxryk.cn

TS:   process.env.HOME
来源：http://dsd.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://iae.fehbvm.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vpl.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://juy.hfpthk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hjf.tanke756.top

[M03] 执行外部命令
来源：http://vgy.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gms.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xuf.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pci.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wsc.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rdt.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wyc.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kal.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://psv.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://mpc.xuetiantiany.cn

Py:   os.getcwd()
来源：http://igq.yvedp.cn

PHP:  getcwd();
来源：http://cbg.yueranfly.top

JS:   process.cwd()
来源：http://wsu.yvedp.cn

TS:   process.cwd()
来源：http://gww.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://xjw.ydzc1.top

Go:   os.Getwd()
来源：http://xlh.sjlbkw.cn

Ruby: Dir.pwd
来源：http://bjc.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://lkg.birdmap.top

[M05] 设置退出码
来源：http://beq.vqdsnc.cn

Py:   sys.exit(1)
来源：http://cap.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://jym.52xcode.cn

JS:   process.exit(1)
来源：http://ccy.zhijiandao.cn

TS:   process.exit(1)
来源：http://qxs.zhiwuduotai.top

Java: System.exit(1)
来源：http://ldy.fehbvm.com

Go:   os.Exit(1)
来源：http://wwi.tarul.cn

Ruby: exit 1
来源：http://big.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cam.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://dea.shanyushiyangtech.top

Py:   print("err", file=sys.stderr)
来源：http://dvy.zhixingplan.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nbu.epnwcf.com

JS:   console.error("err")
来源：http://jck.yvedp.cn

TS:   console.error("err")
来源：http://gjk.316326.xyz

Java: System.err.println("err")
来源：http://pjq.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://erw.haohaochexian.top

Ruby: warn "err"
来源：http://ntm.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://lpc.fktsv.cn

[M07] 判断是否为主入口
来源：http://oio.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://dbc.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iak.fktsv.cn

JS:   require.main === module
来源：http://rxv.hysaishi.cn

TS:   require.main === module
来源：http://hwj.nwbrower.top

Java: public static void main(String[] args)
来源：http://wmb.wangshuangyany.cn

Go:   func main()
来源：http://vvg.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vpy.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://fjr.sufxvd.cn

[M08] 获取系统与运行时信息
来源：http://vfc.dianchejie.cn

Py:   platform.system();  platform.python_version()
来源：http://hsy.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://rix.uphjek.com

JS:   process.platform;  process.version
来源：http://ylt.cqqwz.cn

TS:   process.platform;  process.version
来源：http://pel.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ptz.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://jds.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pob.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ieh.daxiang520.top

================================================================================
来源：http://etd.yfazqb.com

N. 数据结构与算法
来源：http://scf.yj20258888.top

================================================================================
来源：http://kha.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://oai.haohaochexian.top

Py:   bisect.bisect_left(arr, x)
来源：http://tqq.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dac.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ocx.svipenyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zjw.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://xbe.fktsv.cn

Go:   sort.SearchInts(arr, x)
来源：http://jwy.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aek.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://vgi.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://qpu.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://ehe.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aup.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sgu.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://uuz.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bpt.gzhubu.top

Go:   slices.Sort(arr)
来源：http://kay.tarul.cn

Ruby: arr.sort
来源：http://xwa.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bjn.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://ery.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oxu.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://eku.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sjf.gotoacloud.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://llt.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jmi.wangdashe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gcm.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cpu.fzhhl.top

C#:   // 手写递归，或 Array.Sort
来源：http://oqp.tanke756.top

[N04] 斐波那契数列
来源：http://rzg.gotoacloud.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zpq.jiagoushi.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hsy.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mdd.daria6918.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mzq.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sju.andypj.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qqd.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ldh.birdmap.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bny.jqgufenzy.top

[N05] 最大公约数
来源：http://psk.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://vez.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hok.shanyushiyangtech.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dxf.sjlbkw.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kiv.yangfankeji.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uwh.daxiang520.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://psh.tarul.cn

Ruby: a.gcd(b)
来源：http://bsy.sysykeji.top


<!-- 参考信息 -->