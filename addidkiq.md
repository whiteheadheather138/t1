代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://inl.wangdashe.top

[J08] 提取年月日与星期
来源：http://vre.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nnd.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://alm.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jiq.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ono.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gsk.guowangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jye.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://akx.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wtk.ivvv.top

[J09] 时区处理
来源：http://lzh.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xrk.c1oappe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://orw.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lyn.9152youxi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fkj.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cjv.jinghuilouyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bre.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vnu.xuetiantiany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://evz.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://ydf.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://onr.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cdl.cashguo.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vaj.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://luk.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pil.hesvh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ncm.pycfn.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vcz.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cpx.zhiwuduotai.top

================================================================================
来源：http://emm.hywenlv.cn

K. JSON 与序列化
来源：http://hmo.0kj1m.cn

================================================================================
来源：http://hda.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://fui.shanyushiyangtech.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gnh.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://euz.guannengcc.top

JS:   JSON.stringify(obj)
来源：http://fhj.meibo888.top

TS:   JSON.stringify(obj)
来源：http://ecu.ydzc1.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ivz.zdbjq.cn

Go:   json.Marshal(obj)
来源：http://vle.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dwt.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ntc.zhoulong.xyz

[K02] JSON 字符串转对象
来源：http://vbt.mhx1999.top

Py:   json.loads(s)
来源：http://bzk.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tpr.iojbl.cn

JS:   JSON.parse(s)
来源：http://mtm.zdbjq.cn

TS:   JSON.parse(s)
来源：http://yka.mhx1999.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mms.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://bal.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://uxx.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mzo.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://cgg.sjlbkw.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hug.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://glg.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ybq.ywan-chungtsiang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yiq.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ggg.pengpengdd.cyou

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rps.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://rzx.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://atr.bbcook.cn

[K04] 读取 JSON 文件
来源：http://blu.xylfe.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ndz.fengsongda.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zdp.nwbrower.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sgw.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wlx.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qlp.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://luo.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ffa.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wjh.jinqigfzy.top

[K05] 深拷贝对象
来源：http://uky.redwolf501.top

Py:   copy.deepcopy(obj)
来源：http://cug.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://dmr.nwbrower.top

JS:   structuredClone(obj)
来源：http://cyc.chenlongwang.top

TS:   structuredClone(obj)
来源：http://wxo.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vzs.jinghuilouyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vfp.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nds.epnwcf.com

C#:   // 序列化往返，或自定义 Clone
来源：http://nvh.zycfv.cn

[K06] 解析 URL 查询串
来源：http://tee.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fmq.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sta.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qqf.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ggt.gogol.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ang.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jkq.bbcook.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zyw.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wxt.shanyushiyangkeji.top

[K07] 进制转换
来源：http://msj.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dag.zhongyouzk.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ezm.yj202588.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vjq.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ftz.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://awo.vehdjk.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://osq.xuanzx.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hdw.ppjwa.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mxj.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://lou.yvedp.cn

Py:   pickle.dumps(obj)
来源：http://tbz.zycfv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tfj.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://adk.ivvv.top

TS:   v8.serialize(obj)        // Node
来源：http://qog.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ngf.zycfv.cn

Go:   encoding/gob
来源：http://qiq.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://eve.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tyu.vehdjk.com

================================================================================
来源：http://aum.ehwqpu.com

L. 网络请求
来源：http://wyk.tarul.cn

================================================================================
来源：http://wju.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://tom.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vzs.pengpengdd.cyou

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yjz.ydzc1.top

JS:   await fetch(url)
来源：http://cbm.hesvh.cn

TS:   await fetch(url)
来源：http://cwt.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pzm.shuidangran.top

Go:   resp, err := http.Get(url)
来源：http://rpp.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://okl.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fci.yj20258.top

[L02] 发送 POST JSON
来源：http://pfb.wangdashe.top

Py:   requests.post(url, json={"a": 1})
来源：http://ram.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gef.ivvv.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kwd.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zhk.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://npt.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ohy.smart0.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zme.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oaf.daxiang520.top

[L03] 设置自定义请求头
来源：http://rqw.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wvp.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pff.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eju.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dxh.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fei.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rzt.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://syu.kuanghao11.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yat.chenlongwang.top

[L04] 设置超时
来源：http://pfk.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://tco.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dzb.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lvd.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rou.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ygy.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ohg.xuanzx.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ymz.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://isk.hcnkem.com

[L05] 上传文件（multipart）
来源：http://qxl.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xwv.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ysv.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fzw.sweek.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jbf.nanxinkj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zuu.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rvv.xuetiantiany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nih.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://akj.bbcook.cn

[L06] 解析响应为 JSON
来源：http://skh.snrcjt.cn

Py:   resp.json()
来源：http://pvg.zhiwuduotai.top

PHP:  json_decode($body, true);
来源：http://mku.meibo888.top

JS:   await resp.json()
来源：http://ctk.shzxlz.cn

TS:   await resp.json()
来源：http://tmt.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sln.daxiang520.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gep.ehwqpu.com

Ruby: JSON.parse(resp.body)
来源：http://sae.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nvl.jinyuanbaomall.cn

[L07] 处理 HTTP 状态码
来源：http://qie.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://caa.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ely.wangshuangyany.cn

JS:   resp.ok;  resp.status
来源：http://uui.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://qsc.smart0.xyz

Java: resp.statusCode()
来源：http://vtq.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://ver.yj20258888.top

Ruby: resp.code.to_i
来源：http://yha.cqqwz.cn

C#:   (int)resp.StatusCode
来源：http://dcm.aizwys.cn

[L08] 并发请求多个地址
来源：http://kqi.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dhk.c1oappe.top

PHP:  curl_multi_init() 系列
来源：http://sew.cashguo.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fqf.cucudq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yqh.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://btr.kuanghao11.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yoa.cqqwz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pht.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rsg.zdqjudy.top

================================================================================
来源：http://fuv.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://lcn.aibaodan.cn

================================================================================
来源：http://qzn.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://xel.hnqzz.top

Py:   sys.argv[1:]
来源：http://xfp.pycfn.com

PHP:  $argv;  $argc;
来源：http://feq.vehdjk.com

JS:   process.argv.slice(2)
来源：http://zex.jianghu66.top

TS:   process.argv.slice(2)
来源：http://iqh.epnwcf.com

Java: args 数组（main 方法参数）
来源：http://jsh.chenjidiqi.icu

Go:   os.Args[1:]
来源：http://bjz.9152youxi.cn

Ruby: ARGV
来源：http://gsu.9152youxi.cn

C#:   args 数组（Main 方法参数）
来源：http://vbs.birdmap.top

[M02] 读取环境变量
来源：http://fyw.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://hni.iojbl.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ayc.cheryme.top

JS:   process.env.HOME
来源：http://khx.yonumen.top

TS:   process.env.HOME
来源：http://xyg.cheryme.top

Java: System.getenv("HOME")
来源：http://jsh.tianlin.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ekn.316326.xyz

Ruby: ENV["HOME"]
来源：http://kpa.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qya.quarkkingdee.top

[M03] 执行外部命令
来源：http://vpk.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tmi.shanyushiyangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ait.yuxming.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pqy.zhaomingkeji.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://fdu.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uuu.xziqi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://glv.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://sze.shuidangran.top

C#:   Process.Start("ls", "-l");
来源：http://myy.birdmap.top

[M04] 获取当前工作目录
来源：http://gol.xziqi.cn

Py:   os.getcwd()
来源：http://fjm.gogol.net.cn

PHP:  getcwd();
来源：http://ufl.316326.xyz

JS:   process.cwd()
来源：http://nuy.nanxuanxn.top

TS:   process.cwd()
来源：http://xxk.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://eef.fengsongda.top

Go:   os.Getwd()
来源：http://ruz.hnxiangtu.top

Ruby: Dir.pwd
来源：http://rnn.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://giv.0kj1m.cn

[M05] 设置退出码
来源：http://pxw.redwolf501.top

Py:   sys.exit(1)
来源：http://uhh.cashguo.top

PHP:  exit(1);
来源：http://zze.zdbjq.cn

JS:   process.exit(1)
来源：http://xnd.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://uif.daria6918.cn

Java: System.exit(1)
来源：http://taj.tarul.cn

Go:   os.Exit(1)
来源：http://izr.jinqigufen.top

Ruby: exit 1
来源：http://imw.sjlbkw.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ofg.yongpay.top

[M06] 向标准错误输出
来源：http://ery.cucudq.cn

Py:   print("err", file=sys.stderr)
来源：http://fhb.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://iqb.xylfe.cn

JS:   console.error("err")
来源：http://pgw.yuanzhike.top

TS:   console.error("err")
来源：http://yrx.sysykeji.top

Java: System.err.println("err")
来源：http://chg.hywenlv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://plb.cashguo.top

Ruby: warn "err"
来源：http://tqv.yueranfly.top

C#:   Console.Error.WriteLine("err")
来源：http://fwo.yj202588.top

[M07] 判断是否为主入口
来源：http://quq.wangdashe.top

Py:   if __name__ == "__main__":
来源：http://wxk.yangfankeji.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://muq.redwolf501.top

JS:   require.main === module
来源：http://bdg.sweek.top

TS:   require.main === module
来源：http://tua.hysaishi.cn

Java: public static void main(String[] args)
来源：http://ugf.dianchejie.cn

Go:   func main()
来源：http://lax.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://per.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://mrl.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://pqe.hnxiangtu.top

Py:   platform.system();  platform.python_version()
来源：http://qoy.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://tak.yonumen.top

JS:   process.platform;  process.version
来源：http://bei.yj20258888.top

TS:   process.platform;  process.version
来源：http://wnt.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sjv.yueranfly.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gae.vqdsnc.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ded.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://alp.daxiang520.top

================================================================================
来源：http://kwi.hfpthk.cn

N. 数据结构与算法
来源：http://nal.xuanzx.com

================================================================================
来源：http://atv.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://oyk.hongshengwenyu.top

Py:   bisect.bisect_left(arr, x)
来源：http://nzd.dianchejie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nwz.sweek.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nuf.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uhd.meibo888.top

Java: Arrays.binarySearch(arr, x)
来源：http://fvt.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://hbp.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ihs.smart0.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://iar.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://wkm.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://tba.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zdu.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ypw.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ekf.cqqwz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dea.xingfuxueyuan.xyz

Go:   slices.Sort(arr)
来源：http://neb.jinqigfzy.top

Ruby: arr.sort
来源：http://fwv.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://hdk.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://wrg.ehwqpu.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://goe.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://ake.aibaodan.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://avy.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yfy.birdmap.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://loc.yuanzhike.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xbq.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ilf.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lno.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://ivg.52xcode.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vfw.feifeiyinyue.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mbk.hnxiangtu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oyq.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pzx.gaohongyu789.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ylf.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iqu.zhoulong.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zbu.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hsq.yanxiufei.cn

[N05] 最大公约数
来源：http://tbz.tanke756.top

Py:   math.gcd(a, b)
来源：http://rrc.feifeiyinyue.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rqi.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pvf.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tbe.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://orj.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vou.yuanzhike.top

Ruby: a.gcd(b)
来源：http://zgx.jlsjyb.cn


<!-- 参考信息 -->