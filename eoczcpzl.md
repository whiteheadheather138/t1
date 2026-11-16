代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://etp.chenjidiqi.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vex.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ypm.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oxj.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gqs.ydzc1.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lub.hesvh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kcd.gogol.net.cn

[J10] 取今天 / 本月第一天
来源：http://goa.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ceo.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zsu.xuetiantiany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sel.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xag.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lnf.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jvo.zdqjudy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mfa.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://luk.jianghu66.top

================================================================================
来源：http://dcy.smart0.xyz

K. JSON 与序列化
来源：http://ejq.jianghu66.top

================================================================================
来源：http://nia.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://zdv.yangfankeji.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qyw.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://iay.zdbjq.cn

JS:   JSON.stringify(obj)
来源：http://wkf.gaohongyu789.top

TS:   JSON.stringify(obj)
来源：http://dxw.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://met.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://vqp.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://smv.daxiang520.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kgj.vqdsnc.cn

[K02] JSON 字符串转对象
来源：http://awx.hnxiangtu.top

Py:   json.loads(s)
来源：http://zaz.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rdx.ivvv.top

JS:   JSON.parse(s)
来源：http://pjg.cheryme.top

TS:   JSON.parse(s)
来源：http://etc.dianchejie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sly.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://kqd.tarul.cn

Ruby: JSON.parse(s)
来源：http://svy.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://che.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://ziq.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kyw.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lcu.aizwys.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hav.shangyingyoupin.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tjn.xuetiantiany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://agm.zhiwuduotai.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vgy.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fht.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://osb.haohaochexian.top

[K04] 读取 JSON 文件
来源：http://yjv.hywenlv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oau.zhongyouzk.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jma.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cis.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uhh.xingfuxueyuan.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zsp.sufxvd.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qly.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wtk.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://okq.ybcxt.top

[K05] 深拷贝对象
来源：http://uap.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://ohj.tarul.cn

PHP:  unserialize(serialize($obj));
来源：http://pxj.fehbvm.com

JS:   structuredClone(obj)
来源：http://fzs.xinyue.icu

TS:   structuredClone(obj)
来源：http://tea.yfazqb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://ufx.vehdjk.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://byo.cheryme.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nex.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://koh.pengpengdd.cyou

[K06] 解析 URL 查询串
来源：http://esu.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lqg.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qeo.zdbjq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ipt.birdmap.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kxv.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xuh.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qkv.cqqwz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://khn.hnqzz.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zeg.ydzc1.top

[K07] 进制转换
来源：http://ifv.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://skh.fzhhl.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yne.jlsjyb.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lcf.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uwt.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bcj.nwbrower.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mjd.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tsr.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bxg.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://dko.meibo888.top

Py:   pickle.dumps(obj)
来源：http://ppo.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://dre.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://wgq.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://sqs.sufxvd.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ber.hywenlv.cn

Go:   encoding/gob
来源：http://uew.fengsongda.top

Ruby: Marshal.dump(obj)
来源：http://gzm.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bry.meibo888.top

================================================================================
来源：http://lbs.snrcjt.cn

L. 网络请求
来源：http://zjw.bjfxy.top

================================================================================
来源：http://gni.hysaishi.cn

[L01] 发送 GET 请求
来源：http://drq.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://arq.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lcy.guowangkeji.top

JS:   await fetch(url)
来源：http://mol.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://qig.jinqigufen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ozw.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://did.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://osz.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mqr.vehdjk.com

[L02] 发送 POST JSON
来源：http://dmq.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://nxs.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yjh.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xjf.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://evb.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bgt.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ewp.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wsu.zdqjudy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zjt.svipenyu.cn

[L03] 设置自定义请求头
来源：http://ijo.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lap.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nhr.snrcjt.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://syh.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dhr.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gwb.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qkk.ppjwa.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://drd.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cak.cheryme.top

[L04] 设置超时
来源：http://izp.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://unm.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mwa.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cob.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ttl.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://arq.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nbl.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dpm.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ivd.hcnkem.com

[L05] 上传文件（multipart）
来源：http://drh.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cad.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rjq.gogol.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yeq.shzxlz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jqf.ywan-chungtsiang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cnj.snrcjt.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cvw.hcnkem.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bri.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bjm.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://xih.tianlin.xyz

Py:   resp.json()
来源：http://kej.redwolf501.top

PHP:  json_decode($body, true);
来源：http://zuq.tianlin.xyz

JS:   await resp.json()
来源：http://bpp.svipenyu.cn

TS:   await resp.json()
来源：http://cmn.snrcjt.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://who.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fyw.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://rvr.haohaochexian.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://duf.fanxiaobao.xyz

[L07] 处理 HTTP 状态码
来源：http://kzi.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hgm.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fpc.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://grs.ctjpmb.com

TS:   resp.ok;  resp.status
来源：http://xer.fzhhl.top

Java: resp.statusCode()
来源：http://xot.zycfv.cn

Go:   resp.StatusCode
来源：http://toy.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://iwd.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://asg.yvedp.cn

[L08] 并发请求多个地址
来源：http://kva.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kgv.yanxiufei.cn

PHP:  curl_multi_init() 系列
来源：http://xnl.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lzo.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ryq.zhongyouzk.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mhb.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tsn.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fou.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bkz.tanke756.top

================================================================================
来源：http://eoc.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://bji.jinghuilouyu.cn

================================================================================
来源：http://uwt.fktsv.cn

[M01] 读取命令行参数
来源：http://gge.jinghuilouyu.cn

Py:   sys.argv[1:]
来源：http://cyr.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://coq.daria6918.cn

JS:   process.argv.slice(2)
来源：http://tmv.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://yym.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://jvg.yj20258888.top

Go:   os.Args[1:]
来源：http://yoq.yj202588.top

Ruby: ARGV
来源：http://hwi.fehbvm.com

C#:   args 数组（Main 方法参数）
来源：http://bij.ctjpmb.com

[M02] 读取环境变量
来源：http://imw.gzhubu.top

Py:   os.environ.get("HOME")
来源：http://hmi.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fja.ydzc1.top

JS:   process.env.HOME
来源：http://fwk.fzhhl.top

TS:   process.env.HOME
来源：http://lan.hfpthk.cn

Java: System.getenv("HOME")
来源：http://xhk.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lkg.gzhubu.top

Ruby: ENV["HOME"]
来源：http://iah.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pap.ppjwa.cn

[M03] 执行外部命令
来源：http://pzs.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://txq.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iha.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://crl.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wpe.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eyl.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ilb.wangshuangyany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cdz.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://fru.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://jar.daxiang520.top

Py:   os.getcwd()
来源：http://ylc.tarul.cn

PHP:  getcwd();
来源：http://ojy.hesvh.cn

JS:   process.cwd()
来源：http://per.mhx1999.top

TS:   process.cwd()
来源：http://vfl.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://wgs.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://eqs.fehbvm.com

Ruby: Dir.pwd
来源：http://xvo.sufxvd.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tzt.iojbl.cn

[M05] 设置退出码
来源：http://uee.dianchejie.cn

Py:   sys.exit(1)
来源：http://ibc.gotoacloud.top

PHP:  exit(1);
来源：http://pra.tarul.cn

JS:   process.exit(1)
来源：http://jhw.jinqigufen.top

TS:   process.exit(1)
来源：http://whd.chenzaomai.com

Java: System.exit(1)
来源：http://ujw.sysykeji.top

Go:   os.Exit(1)
来源：http://bts.redwolf501.top

Ruby: exit 1
来源：http://mqu.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ste.zhengqikj.top

[M06] 向标准错误输出
来源：http://fbj.sxryk.cn

Py:   print("err", file=sys.stderr)
来源：http://dkv.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ufj.gogol.net.cn

JS:   console.error("err")
来源：http://azb.kuanghao11.cn

TS:   console.error("err")
来源：http://wwz.bjfxy.top

Java: System.err.println("err")
来源：http://zpf.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rvi.hywenlv.cn

Ruby: warn "err"
来源：http://jif.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://lla.yj20258888.top

[M07] 判断是否为主入口
来源：http://qit.sufxvd.cn

Py:   if __name__ == "__main__":
来源：http://vet.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gxf.hcnkem.com

JS:   require.main === module
来源：http://tsj.yj202588.top

TS:   require.main === module
来源：http://fif.xinyue.icu

Java: public static void main(String[] args)
来源：http://pxb.chenlongwang.top

Go:   func main()
来源：http://mly.tian-w.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mpl.cucudq.cn

C#:   static void Main(string[] args)
来源：http://ggd.dianchejie.cn

[M08] 获取系统与运行时信息
来源：http://xps.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://yvj.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://rgo.nanxinkj.top

JS:   process.platform;  process.version
来源：http://mcn.zycfv.cn

TS:   process.platform;  process.version
来源：http://kyi.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bwp.0kj1m.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xhd.zhixingplan.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ozu.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://enp.nwbrower.top

================================================================================
来源：http://eyz.iojbl.cn

N. 数据结构与算法
来源：http://ozq.epnwcf.com

================================================================================
来源：http://zvm.jqgufenzy.top

[N01] 二分查找（有序数组）
来源：http://ics.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://vru.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lke.yfazqb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hli.nanxinkj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yhw.hongshengwenyu.top

Java: Arrays.binarySearch(arr, x)
来源：http://saz.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://zln.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zyp.nwbrower.top

C#:   Array.BinarySearch(arr, x)
来源：http://bar.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://ecf.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://zfc.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qmg.gogol.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cpj.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rhj.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gar.svipenyu.cn

Go:   slices.Sort(arr)
来源：http://agx.quarkkingdee.top

Ruby: arr.sort
来源：http://gci.uphjek.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://vpp.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://ylw.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xha.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://kbm.cucudq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kap.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bwf.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tgc.wangdashe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jkk.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jxq.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://yan.jinqigfzy.top

[N04] 斐波那契数列
来源：http://drj.xuetiantiany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gpp.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ljy.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dgg.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dzy.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ggb.xylfe.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vzq.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pcc.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qur.yfazqb.com

[N05] 最大公约数
来源：http://biv.jinqigufen.top

Py:   math.gcd(a, b)
来源：http://zwh.yj202588.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wqz.guowangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pcf.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fcl.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nwj.ehwqpu.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jqs.zhixingplan.top

Ruby: a.gcd(b)
来源：http://jdz.aizwys.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kos.tianlin.xyz

[N06] 判断回文字符串
来源：http://shc.epnwcf.com

Py:   s == s[::-1]
来源：http://ohm.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://orw.cheryme.top

JS:   s === [...s].reverse().join("")
来源：http://yab.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://lzx.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ywf.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://zkj.ydjk.org.cn

Ruby: s == s.reverse
来源：http://wsr.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://izc.yuanzhike.top

[N07] 两数之和（返回下标）
来源：http://sfv.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pzm.guowangkeji.top


<!-- 参考信息 -->