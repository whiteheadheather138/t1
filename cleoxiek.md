代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://vgd.zhixingplan.top

[J08] 提取年月日与星期
来源：http://acg.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ymd.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qtk.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wrc.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aiw.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://htb.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ecj.aibaodan.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vxt.snrcjt.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gzg.xylfe.cn

[J09] 时区处理
来源：http://ydr.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uof.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dxb.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://boo.nanxuanxn.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iqd.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wog.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zix.uphjek.com

Ruby: Time.now.getlocal("+08:00")
来源：http://fkk.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gxb.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://ceo.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vyb.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lqx.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tak.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zal.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sxw.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://siy.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fwl.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iwk.zhongyouzk.top

================================================================================
来源：http://sii.svipenyu.cn

K. JSON 与序列化
来源：http://ozi.xuanzx.com

================================================================================
来源：http://ivk.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://fzq.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lpv.0kj1m.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dzi.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://rri.yuxming.cn

TS:   JSON.stringify(obj)
来源：http://wqi.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kva.yj20258.top

Go:   json.Marshal(obj)
来源：http://dxm.zdqjudy.top

Ruby: obj.to_json                                     // require "json"
来源：http://dex.guannengcc.top

C#:   JsonSerializer.Serialize(obj)
来源：http://txg.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://ilp.fehbvm.com

Py:   json.loads(s)
来源：http://pqd.chenlongwang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lee.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://yxx.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://mju.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jeg.ehwqpu.com

Go:   json.Unmarshal(data, &v)
来源：http://fea.ydzc1.top

Ruby: JSON.parse(s)
来源：http://rmf.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rpc.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://rfq.sxryk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fig.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wyz.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bmc.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nhw.shangyingyoupin.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gol.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jqr.redwolf501.top

Ruby: JSON.pretty_generate(obj)
来源：http://edm.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jpf.nwbrower.top

[K04] 读取 JSON 文件
来源：http://bzv.xinyue.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iux.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eah.ctjpmb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gxb.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nwt.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://imf.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kve.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qhi.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://svw.smart0.xyz

[K05] 深拷贝对象
来源：http://ukn.wangdashe.top

Py:   copy.deepcopy(obj)
来源：http://vqi.jlsjyb.cn

PHP:  unserialize(serialize($obj));
来源：http://jrp.aizwys.cn

JS:   structuredClone(obj)
来源：http://jya.chenlongwang.top

TS:   structuredClone(obj)
来源：http://kce.snrcjt.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sjp.dashuyun.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mri.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://brt.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vsb.zhoulong.xyz

[K06] 解析 URL 查询串
来源：http://jvi.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pkw.chenjidiqi.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ygt.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://waj.ctjpmb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xzz.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://esz.jqgfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vbd.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://alz.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://usr.ydzc1.top

[K07] 进制转换
来源：http://rze.havefunace.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://czo.jianghu66.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xcy.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://srf.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mrt.uphjek.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ftz.jinyuanbaomall.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zjp.fanxiaobao.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wis.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ffn.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://fwf.shanyushiyangkeji.top

Py:   pickle.dumps(obj)
来源：http://cqp.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lms.yangfankeji.com

JS:   v8.serialize(obj)        // Node
来源：http://wud.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://idp.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tgc.dianchejie.cn

Go:   encoding/gob
来源：http://ipp.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://zbo.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://udh.hongshengwenyu.top

================================================================================
来源：http://dzp.mhx1999.top

L. 网络请求
来源：http://azw.yuxming.cn

================================================================================
来源：http://jwh.smart0.xyz

[L01] 发送 GET 请求
来源：http://fwp.yj20258888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tgu.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rim.jqgufenzy.top

JS:   await fetch(url)
来源：http://hsc.xziqi.cn

TS:   await fetch(url)
来源：http://xsh.yanxiufei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ava.hnqzz.top

Go:   resp, err := http.Get(url)
来源：http://xwp.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://atw.fzhhl.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://eta.fengsongda.top

[L02] 发送 POST JSON
来源：http://aer.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://hnt.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xly.52xcode.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yyt.nanxinkj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dig.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rfp.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dnn.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lpx.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cux.havefunace.top

[L03] 设置自定义请求头
来源：http://zyn.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rbj.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fzt.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qql.yj202588.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ady.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ktx.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kin.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lni.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zwe.zhoulong.xyz

[L04] 设置超时
来源：http://obq.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://ese.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fgd.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://owh.guannengcc.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hdx.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yop.jlsjyb.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vdo.zhijiandao.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nfu.redwolf501.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pjy.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://fyk.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tht.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lmm.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wue.gogol.net.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hbk.jinghuilouyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bjf.chenjidiqi.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jhh.cheryme.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kax.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://igh.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://pdn.nanxinkj.top

Py:   resp.json()
来源：http://zuv.fanxiaobao.xyz

PHP:  json_decode($body, true);
来源：http://tkn.gzhubu.top

JS:   await resp.json()
来源：http://gcg.zhoulong.xyz

TS:   await resp.json()
来源：http://utz.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qvr.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://way.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://nqb.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://min.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://ldp.gotoacloud.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jao.ydjk.org.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ypu.aibaodan.cn

JS:   resp.ok;  resp.status
来源：http://cln.yj202588.top

TS:   resp.ok;  resp.status
来源：http://vpc.nwbrower.top

Java: resp.statusCode()
来源：http://hvr.sweek.top

Go:   resp.StatusCode
来源：http://rbo.shzxlz.cn

Ruby: resp.code.to_i
来源：http://tgz.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://hsc.cashguo.top

[L08] 并发请求多个地址
来源：http://ltc.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wzp.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://dmt.hywenlv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ogx.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lsj.hywenlv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cod.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mvp.cqqwz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ghh.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uwb.hfpthk.cn

================================================================================
来源：http://xuo.pengpengdd.cyou

M. 命令行 / 进程 / 环境
来源：http://iuu.jinqigufen.top

================================================================================
来源：http://ygu.hnxiangtu.top

[M01] 读取命令行参数
来源：http://ktr.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://utx.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://apn.fzhhl.top

JS:   process.argv.slice(2)
来源：http://pkr.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://bec.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://zqp.fzhhl.top

Go:   os.Args[1:]
来源：http://irh.vqdsnc.cn

Ruby: ARGV
来源：http://nzn.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://iob.jianghu66.top

[M02] 读取环境变量
来源：http://bml.redwolf501.top

Py:   os.environ.get("HOME")
来源：http://vfa.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://brc.yj20258888.top

JS:   process.env.HOME
来源：http://ebh.c1oappe.top

TS:   process.env.HOME
来源：http://xoq.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://upq.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zof.xziqi.cn

Ruby: ENV["HOME"]
来源：http://zbl.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://okt.shzxlz.cn

[M03] 执行外部命令
来源：http://fdj.shangyingyoupin.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ggh.chenlongwang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ecb.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://nns.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ycu.chenzaomai.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nbd.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zfz.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lvy.hnqzz.top

C#:   Process.Start("ls", "-l");
来源：http://fjb.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://pbf.aizwys.cn

Py:   os.getcwd()
来源：http://vcy.snrcjt.cn

PHP:  getcwd();
来源：http://zui.ydjk.org.cn

JS:   process.cwd()
来源：http://rot.quarkkingdee.top

TS:   process.cwd()
来源：http://uhk.gogol.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://xza.316326.xyz

Go:   os.Getwd()
来源：http://sni.kuanghao11.cn

Ruby: Dir.pwd
来源：http://sni.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://azh.jlsjyb.cn

[M05] 设置退出码
来源：http://jju.gogol.net.cn

Py:   sys.exit(1)
来源：http://ldf.yanxiufei.cn

PHP:  exit(1);
来源：http://jlk.guowangkeji.top

JS:   process.exit(1)
来源：http://usj.sweek.top

TS:   process.exit(1)
来源：http://cvu.zhengqikj.top

Java: System.exit(1)
来源：http://aqq.cdnleiting.top

Go:   os.Exit(1)
来源：http://ezq.bbcook.cn

Ruby: exit 1
来源：http://cws.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://olv.cucudq.cn

[M06] 向标准错误输出
来源：http://nfj.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://sfp.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://ldm.yvedp.cn

JS:   console.error("err")
来源：http://ouj.fktsv.cn

TS:   console.error("err")
来源：http://mph.yuxming.cn

Java: System.err.println("err")
来源：http://bfu.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vpg.jiagoushi.top

Ruby: warn "err"
来源：http://ktx.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://mhj.xziqi.cn

[M07] 判断是否为主入口
来源：http://eww.9152youxi.cn

Py:   if __name__ == "__main__":
来源：http://vmk.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vyh.jinyuanbaomall.cn

JS:   require.main === module
来源：http://nrb.jiagoushi.top

TS:   require.main === module
来源：http://clf.xziqi.cn

Java: public static void main(String[] args)
来源：http://jue.jinqigfzy.top

Go:   func main()
来源：http://hwu.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qjq.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://qcc.cucudq.cn

[M08] 获取系统与运行时信息
来源：http://roa.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://vyl.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://cwl.vehdjk.com

JS:   process.platform;  process.version
来源：http://aai.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://nkq.jinqigufen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kby.jlsjyb.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nfw.aizwys.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hid.jyoumei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fzu.gaohongyu789.top

================================================================================
来源：http://jhc.sjlbkw.cn

N. 数据结构与算法
来源：http://vdg.sysykeji.top

================================================================================
来源：http://spr.cheryme.top

[N01] 二分查找（有序数组）
来源：http://qbt.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://zqv.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dvn.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gsp.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mpx.gotoacloud.top

Java: Arrays.binarySearch(arr, x)
来源：http://xcj.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://wkl.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pmk.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://vbp.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://gul.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://gsx.sweek.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wix.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zfj.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ouj.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nzi.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://gmn.jianghu66.top

Ruby: arr.sort
来源：http://alo.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://duu.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://mcc.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gnm.gotoacloud.top

PHP:  // 递归实现，或用 usort
来源：http://aqe.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lwg.52xcode.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pst.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pck.aibaodan.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fpb.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dfj.snrcjt.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lgw.zhijiandao.cn

[N04] 斐波那契数列
来源：http://uru.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nyp.hysaishi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fex.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ood.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nhq.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yvj.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://orw.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://efn.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://epl.ehwqpu.com

[N05] 最大公约数
来源：http://ngq.daxiang520.top

Py:   math.gcd(a, b)
来源：http://odd.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://svu.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ssi.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dra.dianchejie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iaw.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://asc.xziqi.cn

Ruby: a.gcd(b)
来源：http://cua.fzhhl.top


<!-- 参考信息 -->