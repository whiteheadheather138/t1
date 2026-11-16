代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://wqk.fktsv.cn

[J08] 提取年月日与星期
来源：http://oji.gotoacloud.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vdr.hesvh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sof.chenlongwang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nmu.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lrz.xuetiantiany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bjr.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jxi.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qqh.sxryk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nfl.yvedp.cn

[J09] 时区处理
来源：http://wla.dashuyun.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://osc.guowangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uko.cashguo.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pzw.zhixingplan.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qnt.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cjz.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://msq.xziqi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://izg.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ezv.yongpay.top

[J10] 取今天 / 本月第一天
来源：http://mdm.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ihi.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nmd.xuanzx.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cms.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ivo.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hac.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://glf.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vhx.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jjx.ywan-chungtsiang.top

================================================================================
来源：http://pcw.shzxlz.cn

K. JSON 与序列化
来源：http://sun.zhixingplan.top

================================================================================
来源：http://tzu.zhijiandao.cn

[K01] 对象转 JSON 字符串
来源：http://tqi.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://avt.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vta.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://urh.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://toi.jinqigufen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://obe.ybcxt.top

Go:   json.Marshal(obj)
来源：http://qlu.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://ksl.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://anh.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://iif.chenjidiqi.icu

Py:   json.loads(s)
来源：http://amw.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nat.jinqigfzy.top

JS:   JSON.parse(s)
来源：http://aaz.zycfv.cn

TS:   JSON.parse(s)
来源：http://yhm.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://txt.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://nqb.birdmap.top

Ruby: JSON.parse(s)
来源：http://fac.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kus.tian-w.cn

[K03] JSON 美化输出（带缩进）
来源：http://frf.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cex.quarkkingdee.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ual.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://nap.jqgufenzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://snz.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xtk.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xrn.ppjwa.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lzu.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qmr.jqgfzy.top

[K04] 读取 JSON 文件
来源：http://euq.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lxw.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zin.yangfankeji.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kjj.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vmv.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://amw.c1oappe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://avx.wangshuangyany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jim.hammf.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fow.hywenlv.cn

[K05] 深拷贝对象
来源：http://yth.zhoulong.xyz

Py:   copy.deepcopy(obj)
来源：http://qmr.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://odv.fktsv.cn

JS:   structuredClone(obj)
来源：http://ogj.zhixingplan.top

TS:   structuredClone(obj)
来源：http://sdv.yanxiufei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cjy.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pui.sysykeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jvz.shangyingyoupin.top

C#:   // 序列化往返，或自定义 Clone
来源：http://phk.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://cds.shzxlz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gto.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ssn.nwbrower.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fnr.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ckv.aibaodan.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nlg.redwolf501.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ktd.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kaq.jiagoushi.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gvx.shuidangran.top

[K07] 进制转换
来源：http://zxx.aizwys.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ywz.zdbjq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cjo.zycfv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lhg.tian-w.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cid.pycfn.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hue.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jst.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cfa.cheryme.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xoi.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://qgu.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://eoh.feifeiyinyue.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yzq.xuanzx.com

JS:   v8.serialize(obj)        // Node
来源：http://qeo.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://gze.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xcp.sufxvd.cn

Go:   encoding/gob
来源：http://dhh.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://qnb.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://moo.yj20258.top

================================================================================
来源：http://faj.wangshuangyany.cn

L. 网络请求
来源：http://orx.dianchejie.cn

================================================================================
来源：http://zxa.zhengqikj.top

[L01] 发送 GET 请求
来源：http://qqd.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://otd.jinghuilouyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nkt.jiagoushi.top

JS:   await fetch(url)
来源：http://ewn.shuidangran.top

TS:   await fetch(url)
来源：http://yka.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mlc.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://swf.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dvf.birdmap.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fez.hammf.cn

[L02] 发送 POST JSON
来源：http://rco.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wtf.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jlg.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tap.zhaomingkeji.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nwc.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wvg.sxryk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mok.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://usq.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kwq.shanyushiyangkeji.top

[L03] 设置自定义请求头
来源：http://sci.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rnd.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://znf.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rbt.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tuq.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jpj.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://upi.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qzc.hnxiangtu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nso.52xcode.cn

[L04] 设置超时
来源：http://hyg.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://voi.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gjs.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yyr.ehwqpu.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bno.quarkkingdee.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vqf.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eit.pengpengdd.cyou

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cbx.hongshengwenyu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uws.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://hhu.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mtx.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xqj.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ydx.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zol.chenjidiqi.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://unr.nanxuanxn.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lba.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pia.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ytp.birdmap.top

[L06] 解析响应为 JSON
来源：http://tyl.hnxiangtu.top

Py:   resp.json()
来源：http://zun.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://zgx.sxryk.cn

JS:   await resp.json()
来源：http://bdz.yuanzhike.top

TS:   await resp.json()
来源：http://ivl.316326.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oxs.hywenlv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://amu.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://jrn.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hit.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://mxw.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xgf.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zqi.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://ilo.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://pqk.hysaishi.cn

Java: resp.statusCode()
来源：http://qtf.xinyue.icu

Go:   resp.StatusCode
来源：http://mzt.zycfv.cn

Ruby: resp.code.to_i
来源：http://pxz.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://flc.hywenlv.cn

[L08] 并发请求多个地址
来源：http://pny.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qsr.birdmap.top

PHP:  curl_multi_init() 系列
来源：http://tmz.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sgh.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oct.ydzc1.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bnq.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sqz.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kkk.nwbrower.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gxd.epnwcf.com

================================================================================
来源：http://sie.wangdashe.top

M. 命令行 / 进程 / 环境
来源：http://var.52xcode.cn

================================================================================
来源：http://rab.yj202588.top

[M01] 读取命令行参数
来源：http://pbh.aizwys.cn

Py:   sys.argv[1:]
来源：http://ikw.xziqi.cn

PHP:  $argv;  $argc;
来源：http://adp.fehbvm.com

JS:   process.argv.slice(2)
来源：http://vmb.wangdashe.top

TS:   process.argv.slice(2)
来源：http://lem.316326.xyz

Java: args 数组（main 方法参数）
来源：http://jhl.jlsjyb.cn

Go:   os.Args[1:]
来源：http://vzp.birdmap.top

Ruby: ARGV
来源：http://vbr.shuidangran.top

C#:   args 数组（Main 方法参数）
来源：http://rcp.zdbjq.cn

[M02] 读取环境变量
来源：http://lzg.meibo888.top

Py:   os.environ.get("HOME")
来源：http://rzj.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hly.daxiang520.top

JS:   process.env.HOME
来源：http://bef.svipenyu.cn

TS:   process.env.HOME
来源：http://zwo.jinqigufen.top

Java: System.getenv("HOME")
来源：http://qbc.ydzc1.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://twl.0kj1m.cn

Ruby: ENV["HOME"]
来源：http://jdj.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qjn.jlsjyb.cn

[M03] 执行外部命令
来源：http://ara.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dyz.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kxb.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dkw.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://uhd.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uxg.sxryk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://egv.hcnkem.com

Ruby: system("ls -l");  `ls -l`
来源：http://gys.jinqigfzy.top

C#:   Process.Start("ls", "-l");
来源：http://kkd.shuidangran.top

[M04] 获取当前工作目录
来源：http://cfs.cucudq.cn

Py:   os.getcwd()
来源：http://zgj.jlsjyb.cn

PHP:  getcwd();
来源：http://jek.ywan-chungtsiang.top

JS:   process.cwd()
来源：http://lpy.xuetiantiany.cn

TS:   process.cwd()
来源：http://fye.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://rur.fengsongda.top

Go:   os.Getwd()
来源：http://gen.ydjk.org.cn

Ruby: Dir.pwd
来源：http://zdq.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://sfo.jinghuilouyu.cn

[M05] 设置退出码
来源：http://odp.hesvh.cn

Py:   sys.exit(1)
来源：http://glg.fzhhl.top

PHP:  exit(1);
来源：http://jal.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://rtp.ehwqpu.com

TS:   process.exit(1)
来源：http://jny.dashuyun.cn

Java: System.exit(1)
来源：http://vpv.shuidangran.top

Go:   os.Exit(1)
来源：http://fid.gzhubu.top

Ruby: exit 1
来源：http://cfl.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jmr.tanke756.top

[M06] 向标准错误输出
来源：http://icx.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://bww.ppjwa.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hzb.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://kuf.feifeiyinyue.top

TS:   console.error("err")
来源：http://kpv.jiagoushi.top

Java: System.err.println("err")
来源：http://mjp.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fax.zhijiandao.cn

Ruby: warn "err"
来源：http://ygg.guannengcc.top

C#:   Console.Error.WriteLine("err")
来源：http://gok.yonumen.top

[M07] 判断是否为主入口
来源：http://hho.yvedp.cn

Py:   if __name__ == "__main__":
来源：http://ssw.hfpthk.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://snw.yj202588.top

JS:   require.main === module
来源：http://wgu.ydzc1.top

TS:   require.main === module
来源：http://bai.0kj1m.cn

Java: public static void main(String[] args)
来源：http://xux.hnqzz.top

Go:   func main()
来源：http://kgu.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hrd.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://ovs.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://rev.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://nxt.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://elu.yuanzhike.top

JS:   process.platform;  process.version
来源：http://lny.gzhubu.top

TS:   process.platform;  process.version
来源：http://kxi.zycfv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://knx.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yyz.zycfv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wta.9152youxi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zwm.jianghu66.top

================================================================================
来源：http://euf.ivvv.top

N. 数据结构与算法
来源：http://arx.jqgufenzy.top

================================================================================
来源：http://kwk.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://fyg.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://zvf.yangfankeji.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sje.sufxvd.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wdc.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kvt.hcnkem.com

Java: Arrays.binarySearch(arr, x)
来源：http://kpd.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://cuh.haohaochexian.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fcc.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://thx.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://mjk.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://ets.sweek.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cpi.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xun.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rvx.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://anf.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://ijy.shzxlz.cn

Ruby: arr.sort
来源：http://dwu.cashguo.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jtn.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://wzf.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fbg.xuetiantiany.cn

PHP:  // 递归实现，或用 usort
来源：http://gfk.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mdp.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://opv.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://slt.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lwx.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rpj.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://mfn.andypj.xyz

[N04] 斐波那契数列
来源：http://gpn.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vxc.uphjek.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://skn.shangyingyoupin.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oym.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hpm.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vsi.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ccp.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wwt.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://euw.jqgufenzy.top

[N05] 最大公约数
来源：http://hiy.zhaomingkeji.xyz

Py:   math.gcd(a, b)
来源：http://hty.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lji.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bxi.zhaomingkeji.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nay.tarul.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://obz.zhongyouzk.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kql.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://vsm.yfazqb.com


<!-- 参考信息 -->