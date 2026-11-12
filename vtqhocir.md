代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jaq.daxiang520.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oib.bbcook.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lwm.uphjek.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bef.zdqjudy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kqa.jiagoushi.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dof.chenjidiqi.icu

[J09] 时区处理
来源：http://pvt.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dpg.tian-w.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://avy.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lyu.sufxvd.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kvr.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tpq.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fzl.sufxvd.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bxn.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://afi.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://yrj.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nan.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fhn.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dck.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ehe.yfazqb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uet.cucudq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://txm.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qtt.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bnf.jlsjyb.cn

================================================================================
来源：http://wzf.ydzc1.top

K. JSON 与序列化
来源：http://hau.zhiwuduotai.top

================================================================================
来源：http://asy.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://gny.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://quy.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xdv.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://zse.ydjk.org.cn

TS:   JSON.stringify(obj)
来源：http://bzf.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ike.jqgfzy.top

Go:   json.Marshal(obj)
来源：http://dqx.yj202588.top

Ruby: obj.to_json                                     // require "json"
来源：http://grs.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ugv.fehbvm.com

[K02] JSON 字符串转对象
来源：http://zpk.nwbrower.top

Py:   json.loads(s)
来源：http://tpx.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lqi.sufxvd.cn

JS:   JSON.parse(s)
来源：http://llp.wangdashe.top

TS:   JSON.parse(s)
来源：http://lrl.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hij.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://avb.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://yhs.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pwj.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://evr.ppjwa.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ypn.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qfs.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uug.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dlo.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fwn.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iqn.tian-w.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fzw.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://byn.yj20258.top

[K04] 读取 JSON 文件
来源：http://lxg.jlsjyb.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://inm.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hqn.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vam.fzhhl.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qpj.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hpp.9152youxi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lmq.wangshuangyany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gmz.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hrt.jyoumei.cn

[K05] 深拷贝对象
来源：http://esw.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://pxw.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://alb.cqqwz.cn

JS:   structuredClone(obj)
来源：http://jap.gaohongyu789.top

TS:   structuredClone(obj)
来源：http://hqb.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://okv.nwbrower.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://teh.feifeiyinyue.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zsz.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://aaj.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://syz.kuanghao11.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rcw.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uag.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pkq.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ijw.gogol.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://txb.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qob.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://clo.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://edc.jinyuanbaomall.cn

[K07] 进制转换
来源：http://tli.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zou.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tlr.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tcp.zhixingplan.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wqy.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ulw.dianchejie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mtb.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dmr.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fxg.havefunace.top

[K08] 二进制序列化（非 JSON）
来源：http://fwa.andypj.xyz

Py:   pickle.dumps(obj)
来源：http://idj.wangshuangyany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ouy.havefunace.top

JS:   v8.serialize(obj)        // Node
来源：http://daq.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://nhe.zhengqikj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://opk.zhongyouzk.top

Go:   encoding/gob
来源：http://kqh.svipenyu.cn

Ruby: Marshal.dump(obj)
来源：http://jkt.zhaomingkeji.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://abe.hnxiangtu.top

================================================================================
来源：http://mbx.cashguo.top

L. 网络请求
来源：http://mxz.ybcxt.top

================================================================================
来源：http://zjz.316326.xyz

[L01] 发送 GET 请求
来源：http://hby.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xis.xylfe.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xgb.tarul.cn

JS:   await fetch(url)
来源：http://efw.jqgufenzy.top

TS:   await fetch(url)
来源：http://ajq.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zlb.zhongyouzk.top

Go:   resp, err := http.Get(url)
来源：http://lxm.chenjidiqi.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://enc.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hiy.tian-w.cn

[L02] 发送 POST JSON
来源：http://gkt.9152youxi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lak.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iwu.zhijiandao.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bka.tarul.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://evu.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ise.fanxiaobao.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://enk.ctjpmb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://upy.iojbl.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lhc.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://ims.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eay.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xfj.yanxiufei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kjk.hcnkem.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uul.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uft.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ccs.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dba.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mnw.andypj.xyz

[L04] 设置超时
来源：http://qcg.bjfxy.top

Py:   requests.get(url, timeout=5)
来源：http://tag.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cxx.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gju.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eis.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oay.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cqn.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pkk.wangshuangyany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zml.meibo888.top

[L05] 上传文件（multipart）
来源：http://xcq.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yhp.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rqk.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rmj.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cnd.sweek.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rtp.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rvw.316326.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jia.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eos.cheryme.top

[L06] 解析响应为 JSON
来源：http://eae.gaohongyu789.top

Py:   resp.json()
来源：http://dee.hnqzz.top

PHP:  json_decode($body, true);
来源：http://auc.xylfe.cn

JS:   await resp.json()
来源：http://srq.daria6918.cn

TS:   await resp.json()
来源：http://iym.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rhe.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uif.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://xqv.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pqq.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://kye.cashguo.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jly.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rwi.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://xww.zycfv.cn

TS:   resp.ok;  resp.status
来源：http://jqi.zhengqikj.top

Java: resp.statusCode()
来源：http://sjh.hcnkem.com

Go:   resp.StatusCode
来源：http://hlm.vqdsnc.cn

Ruby: resp.code.to_i
来源：http://cdv.haohaochexian.top

C#:   (int)resp.StatusCode
来源：http://ijk.mhx1999.top

[L08] 并发请求多个地址
来源：http://ylf.vehdjk.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://osf.chenjidiqi.icu

PHP:  curl_multi_init() 系列
来源：http://vmj.fanxiaobao.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ulu.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vos.fanxiaobao.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cnk.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://chb.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jlt.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xno.bbcook.cn

================================================================================
来源：http://big.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://aae.sufxvd.cn

================================================================================
来源：http://jqw.mhx1999.top

[M01] 读取命令行参数
来源：http://fiz.xingfuxueyuan.xyz

Py:   sys.argv[1:]
来源：http://ctz.zdqjudy.top

PHP:  $argv;  $argc;
来源：http://qce.fehbvm.com

JS:   process.argv.slice(2)
来源：http://vdw.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://nnv.zhixingplan.top

Java: args 数组（main 方法参数）
来源：http://veq.gzhubu.top

Go:   os.Args[1:]
来源：http://fwy.zhijiandao.cn

Ruby: ARGV
来源：http://zrh.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://mcp.jyoumei.cn

[M02] 读取环境变量
来源：http://kru.hnxiangtu.top

Py:   os.environ.get("HOME")
来源：http://fdg.zhongyouzk.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rxm.xinyue.icu

JS:   process.env.HOME
来源：http://avf.havefunace.top

TS:   process.env.HOME
来源：http://whg.hnqzz.top

Java: System.getenv("HOME")
来源：http://fcr.guannengcc.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pqu.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://cvf.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mkt.tian-w.cn

[M03] 执行外部命令
来源：http://fmd.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ycv.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://egr.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://oif.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://yhb.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kal.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xrj.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://vnq.ctjpmb.com

C#:   Process.Start("ls", "-l");
来源：http://cvd.sufxvd.cn

[M04] 获取当前工作目录
来源：http://lhd.jyoumei.cn

Py:   os.getcwd()
来源：http://drs.zhoulong.xyz

PHP:  getcwd();
来源：http://pvt.shangyingyoupin.top

JS:   process.cwd()
来源：http://ejj.nanxinkj.top

TS:   process.cwd()
来源：http://kzk.hysaishi.cn

Java: Path.of("").toAbsolutePath()
来源：http://xym.kuanghao11.cn

Go:   os.Getwd()
来源：http://vcb.uphjek.com

Ruby: Dir.pwd
来源：http://wcq.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://zxk.zhiwuduotai.top

[M05] 设置退出码
来源：http://abs.ywan-chungtsiang.top

Py:   sys.exit(1)
来源：http://qyf.zdqjudy.top

PHP:  exit(1);
来源：http://hei.dianchejie.cn

JS:   process.exit(1)
来源：http://aas.sufxvd.cn

TS:   process.exit(1)
来源：http://ycr.yj20258888.top

Java: System.exit(1)
来源：http://hpz.hammf.cn

Go:   os.Exit(1)
来源：http://zdo.xuetiantiany.cn

Ruby: exit 1
来源：http://cte.zdbjq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wfa.jinqigfzy.top

[M06] 向标准错误输出
来源：http://xux.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://gqj.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lkf.yueranfly.top

JS:   console.error("err")
来源：http://fmj.daxiang520.top

TS:   console.error("err")
来源：http://zwy.yuanzhike.top

Java: System.err.println("err")
来源：http://hmg.yueranfly.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://boz.yj20258.top

Ruby: warn "err"
来源：http://cha.zhoulong.xyz

C#:   Console.Error.WriteLine("err")
来源：http://rnr.fktsv.cn

[M07] 判断是否为主入口
来源：http://kky.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://pfm.hnxiangtu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fqc.hcnkem.com

JS:   require.main === module
来源：http://vws.hongshengwenyu.top

TS:   require.main === module
来源：http://lao.shangyingyoupin.top

Java: public static void main(String[] args)
来源：http://gys.zdqjudy.top

Go:   func main()
来源：http://vtj.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xot.daria6918.cn

C#:   static void Main(string[] args)
来源：http://qwb.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://ext.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://mlw.daxiang520.top

PHP:  PHP_OS;  phpversion();
来源：http://idm.bbcook.cn

JS:   process.platform;  process.version
来源：http://zvp.gotoacloud.top

TS:   process.platform;  process.version
来源：http://lti.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pkk.yvedp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wgr.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kpi.zycfv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zbt.cheryme.top

================================================================================
来源：http://llb.xziqi.cn

N. 数据结构与算法
来源：http://swr.zhengqikj.top

================================================================================
来源：http://bbt.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://pch.zycfv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qjn.smart0.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eph.zhongyouzk.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xwd.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jxz.jinqigufen.top

Java: Arrays.binarySearch(arr, x)
来源：http://rur.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://usg.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mus.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ftk.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://rqg.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://yfo.kuanghao11.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ynz.xziqi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ddq.andypj.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://ffx.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://drn.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://rkm.hongshengwenyu.top

Ruby: arr.sort
来源：http://kmn.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://bjc.shangyingyoupin.top

[N03] 快速排序（分治示例）
来源：http://ipx.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://glk.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://izh.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://akl.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xyy.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kzc.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nrh.yuanzhike.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hhp.ywan-chungtsiang.top

C#:   // 手写递归，或 Array.Sort
来源：http://hvg.hysaishi.cn

[N04] 斐波那契数列
来源：http://znw.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ecp.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zvm.tanke756.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://igr.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://alr.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cve.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ecd.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dsw.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yad.redwolf501.top

[N05] 最大公约数
来源：http://gml.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://zos.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rvm.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blo.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dpe.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jig.shzxlz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zvx.aizwys.cn

Ruby: a.gcd(b)
来源：http://loa.jinqigfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tcx.jinqigufen.top

[N06] 判断回文字符串
来源：http://vle.bjfxy.top

Py:   s == s[::-1]
来源：http://acy.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://pij.hcnkem.com


<!-- 参考信息 -->