代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://ges.0kj1m.cn

[J08] 提取年月日与星期
来源：http://lxy.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vyg.52xcode.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://okh.jinyuanbaomall.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lns.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mic.pengpengdd.cyou

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lah.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ybc.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bcy.gogol.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://idw.daxiang520.top

[J09] 时区处理
来源：http://ztd.zhoulong.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ekx.guannengcc.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yya.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gjy.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jaf.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://atd.sweek.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bat.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://mup.vehdjk.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gpb.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://cax.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://qeb.aizwys.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ehc.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iwh.xuanzx.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cwg.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jal.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ype.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hkj.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://neo.jinqigufen.top

================================================================================
来源：http://hrv.bjfxy.top

K. JSON 与序列化
来源：http://ylo.yanxiufei.cn

================================================================================
来源：http://uyh.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://hja.guowangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jzt.kuanghao11.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yaf.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://bjp.zhijiandao.cn

TS:   JSON.stringify(obj)
来源：http://dxo.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jmw.shangyingyoupin.top

Go:   json.Marshal(obj)
来源：http://nwb.xziqi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://orm.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bps.xinyue.icu

[K02] JSON 字符串转对象
来源：http://lum.zdqjudy.top

Py:   json.loads(s)
来源：http://huh.yj20258.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jwz.cqqwz.cn

JS:   JSON.parse(s)
来源：http://lgu.fehbvm.com

TS:   JSON.parse(s)
来源：http://cip.iojbl.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bkz.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://dup.cucudq.cn

Ruby: JSON.parse(s)
来源：http://pqf.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hdx.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://bmc.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wmj.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ien.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://imz.shanyushiyangtech.top

TS:   JSON.stringify(obj, null, 2)
来源：http://adk.nanxuanxn.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gbf.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ssi.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://fgx.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lkq.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://lfm.zdqjudy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cfm.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lcq.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dht.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zol.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dek.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kvf.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tqs.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hwx.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://gpp.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://xfe.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://yhi.hywenlv.cn

JS:   structuredClone(obj)
来源：http://fhe.ydjk.org.cn

TS:   structuredClone(obj)
来源：http://joj.yfazqb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://vme.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kis.jqgfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nyo.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ewn.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://doe.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iar.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qeb.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ysa.zhijiandao.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hhf.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nxx.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rny.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://niv.fengsongda.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ikn.yanxiufei.cn

[K07] 进制转换
来源：http://kir.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xob.haohaochexian.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lzu.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yjx.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cuo.shanyushiyangtech.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nlz.xinyue.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qmj.hfpthk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hdj.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://syz.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://elf.chenzaomai.com

Py:   pickle.dumps(obj)
来源：http://huf.jqgufenzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sys.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://eas.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://llg.yuxming.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://thn.daxiang520.top

Go:   encoding/gob
来源：http://hyg.xinyue.icu

Ruby: Marshal.dump(obj)
来源：http://buw.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tdx.ywan-chungtsiang.top

================================================================================
来源：http://abd.zhixingplan.top

L. 网络请求
来源：http://xcd.ehwqpu.com

================================================================================
来源：http://lsa.hfpthk.cn

[L01] 发送 GET 请求
来源：http://onp.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://loe.xuanzx.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bcw.chenjidiqi.icu

JS:   await fetch(url)
来源：http://kqx.chenzaomai.com

TS:   await fetch(url)
来源：http://knj.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bdr.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://fjc.ydjk.org.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qkx.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tse.jiagoushi.top

[L02] 发送 POST JSON
来源：http://evp.chenlongwang.top

Py:   requests.post(url, json={"a": 1})
来源：http://mxo.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tym.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eli.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bqz.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://srx.hysaishi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lgb.tanke756.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://syi.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nkv.hesvh.cn

[L03] 设置自定义请求头
来源：http://doq.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oyd.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://htv.xinyue.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oap.fzhhl.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ilb.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qbw.jinqigfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tso.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://quy.mhx1999.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xxv.cqqwz.cn

[L04] 设置超时
来源：http://hnp.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://tip.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ext.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://syq.xylfe.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://spd.zhaomingkeji.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mir.redwolf501.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kva.snrcjt.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bzt.tianlin.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wwx.shanyushiyangkeji.top

[L05] 上传文件（multipart）
来源：http://njz.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ufe.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fxg.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://not.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bwa.fanxiaobao.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qnb.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tpm.ctjpmb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qgy.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qqq.daria6918.cn

[L06] 解析响应为 JSON
来源：http://ryi.ydzc1.top

Py:   resp.json()
来源：http://uzb.bjfxy.top

PHP:  json_decode($body, true);
来源：http://sow.sxryk.cn

JS:   await resp.json()
来源：http://gko.jinqigfzy.top

TS:   await resp.json()
来源：http://ezu.chenlongwang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rkf.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cjh.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://zdb.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cks.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://bde.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xsa.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://znz.yvedp.cn

JS:   resp.ok;  resp.status
来源：http://yow.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://djy.aizwys.cn

Java: resp.statusCode()
来源：http://wgd.yangfankeji.com

Go:   resp.StatusCode
来源：http://oki.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://gtt.jinyuanbaomall.cn

C#:   (int)resp.StatusCode
来源：http://dxe.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://qie.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ecs.jinqigufen.top

PHP:  curl_multi_init() 系列
来源：http://ffq.xylfe.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lbf.sxryk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ufy.ehwqpu.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nwf.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://swp.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xai.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ysf.tarul.cn

================================================================================
来源：http://zwt.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://uaa.hnxiangtu.top

================================================================================
来源：http://ghl.shuidangran.top

[M01] 读取命令行参数
来源：http://jgb.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://rjq.gogol.net.cn

PHP:  $argv;  $argc;
来源：http://eks.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://jtt.xuetiantiany.cn

TS:   process.argv.slice(2)
来源：http://igp.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://gxw.xziqi.cn

Go:   os.Args[1:]
来源：http://gnb.tanke756.top

Ruby: ARGV
来源：http://kbz.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://mki.yanxiufei.cn

[M02] 读取环境变量
来源：http://wtc.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://azy.fanxiaobao.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://brs.jqgufenzy.top

JS:   process.env.HOME
来源：http://pcu.jyoumei.cn

TS:   process.env.HOME
来源：http://hyw.hongshengwenyu.top

Java: System.getenv("HOME")
来源：http://xpa.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hpc.aibaodan.cn

Ruby: ENV["HOME"]
来源：http://koh.jinqigufen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hfo.hysaishi.cn

[M03] 执行外部命令
来源：http://dkd.0kj1m.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://amz.bbcook.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gtv.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lry.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://iur.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iev.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://myr.shangyingyoupin.top

Ruby: system("ls -l");  `ls -l`
来源：http://tin.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://efx.cashguo.top

[M04] 获取当前工作目录
来源：http://ojv.jyoumei.cn

Py:   os.getcwd()
来源：http://zgt.shanyushiyangtech.top

PHP:  getcwd();
来源：http://pci.hcnkem.com

JS:   process.cwd()
来源：http://mzl.tian-w.cn

TS:   process.cwd()
来源：http://vce.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://lfk.fzhhl.top

Go:   os.Getwd()
来源：http://pzl.andypj.xyz

Ruby: Dir.pwd
来源：http://qas.cdnleiting.top

C#:   Directory.GetCurrentDirectory()
来源：http://ytd.zhixingplan.top

[M05] 设置退出码
来源：http://ywz.fanxiaobao.xyz

Py:   sys.exit(1)
来源：http://keq.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://pjp.yvedp.cn

JS:   process.exit(1)
来源：http://eqj.bbcook.cn

TS:   process.exit(1)
来源：http://jsh.jianghu66.top

Java: System.exit(1)
来源：http://wfa.daxiang520.top

Go:   os.Exit(1)
来源：http://xzo.shuidangran.top

Ruby: exit 1
来源：http://dxj.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bmg.dianchejie.cn

[M06] 向标准错误输出
来源：http://oar.vqdsnc.cn

Py:   print("err", file=sys.stderr)
来源：http://znx.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gsk.epnwcf.com

JS:   console.error("err")
来源：http://odt.zhijiandao.cn

TS:   console.error("err")
来源：http://hfw.zhixingplan.top

Java: System.err.println("err")
来源：http://wwl.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yno.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://mtz.shanyushiyangtech.top

C#:   Console.Error.WriteLine("err")
来源：http://cwg.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://iyd.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://imq.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fmi.bjfxy.top

JS:   require.main === module
来源：http://fnr.svipenyu.cn

TS:   require.main === module
来源：http://jer.ywan-chungtsiang.top

Java: public static void main(String[] args)
来源：http://ypj.sufxvd.cn

Go:   func main()
来源：http://uch.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fti.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://efr.xuanzx.com

[M08] 获取系统与运行时信息
来源：http://xmu.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://ely.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://azq.chenjidiqi.icu

JS:   process.platform;  process.version
来源：http://kzi.vehdjk.com

TS:   process.platform;  process.version
来源：http://wtw.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yod.birdmap.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ugg.tian-w.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ihg.jiagoushi.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://coe.aibaodan.cn

================================================================================
来源：http://ied.ctjpmb.com

N. 数据结构与算法
来源：http://gzs.jyoumei.cn

================================================================================
来源：http://qia.svipenyu.cn

[N01] 二分查找（有序数组）
来源：http://rzo.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ofh.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dpy.iojbl.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lwb.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tgy.sysykeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://nbx.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://wpx.jinqigufen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ijb.svipenyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pdx.xuanzx.com

[N02] 排序（工程实践用内置实现）
来源：http://zbs.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://eso.zhiwuduotai.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://noe.shanyushiyangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ncx.mhx1999.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wgs.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ckj.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://jjr.jiagoushi.top

Ruby: arr.sort
来源：http://lzh.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://iyl.cqqwz.cn

[N03] 快速排序（分治示例）
来源：http://vrj.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lbi.ctjpmb.com

PHP:  // 递归实现，或用 usort
来源：http://fxb.0kj1m.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://efq.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://key.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ozs.hammf.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wxm.tian-w.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xps.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://tsp.jqgfzy.top

[N04] 斐波那契数列
来源：http://jjw.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dyh.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jir.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kxf.cucudq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://njv.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ytg.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dqr.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://khc.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lzh.iojbl.cn

[N05] 最大公约数
来源：http://maz.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://akj.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://awc.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rjj.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uqi.ppjwa.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vhm.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dpd.wangshuangyany.cn

Ruby: a.gcd(b)
来源：http://qok.zycfv.cn


<!-- 参考信息 -->