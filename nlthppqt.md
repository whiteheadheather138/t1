代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://fcn.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://sng.ydjk.org.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mia.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lzi.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ogu.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tce.cashguo.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zru.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://olz.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mah.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rha.52xcode.cn

[J09] 时区处理
来源：http://nwh.ppjwa.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zxc.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qal.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kkm.quarkkingdee.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ktm.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bfr.fanxiaobao.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://euc.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://psd.shanyushiyangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nxo.zycfv.cn

[J10] 取今天 / 本月第一天
来源：http://wpy.shanyushiyangtech.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ozq.vqdsnc.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pfk.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://edk.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ste.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mgm.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dwc.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mbr.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ltu.zhiwuduotai.top

================================================================================
来源：http://hik.bjfxy.top

K. JSON 与序列化
来源：http://ayw.guowangkeji.top

================================================================================
来源：http://lvj.uphjek.com

[K01] 对象转 JSON 字符串
来源：http://wvz.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xcf.c1oappe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bst.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://keu.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://lqw.sweek.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qul.gzhubu.top

Go:   json.Marshal(obj)
来源：http://ppk.9152youxi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jak.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://evw.vehdjk.com

[K02] JSON 字符串转对象
来源：http://ujk.ydzc1.top

Py:   json.loads(s)
来源：http://arh.smart0.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://stt.hysaishi.cn

JS:   JSON.parse(s)
来源：http://bcn.shanyushiyangkeji.top

TS:   JSON.parse(s)
来源：http://kdx.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bay.sysykeji.top

Go:   json.Unmarshal(data, &v)
来源：http://jtd.ywan-chungtsiang.top

Ruby: JSON.parse(s)
来源：http://zms.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gjb.zdqjudy.top

[K03] JSON 美化输出（带缩进）
来源：http://uot.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ovu.ppjwa.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hvs.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uod.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wfk.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mhl.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hpq.yanxiufei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tzo.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fkp.guowangkeji.top

[K04] 读取 JSON 文件
来源：http://wzi.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rsp.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gvv.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fec.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jij.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jgh.haohaochexian.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hef.chenlongwang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://slh.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kip.shuidangran.top

[K05] 深拷贝对象
来源：http://sgt.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://zea.tian-w.cn

PHP:  unserialize(serialize($obj));
来源：http://ujh.jqgfzy.top

JS:   structuredClone(obj)
来源：http://zlu.tarul.cn

TS:   structuredClone(obj)
来源：http://ppe.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://gag.snrcjt.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uyc.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xyp.ywan-chungtsiang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dma.xziqi.cn

[K06] 解析 URL 查询串
来源：http://mhs.wangdashe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://suc.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nkb.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://waq.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tbs.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uey.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://noh.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pob.andypj.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ext.shanyushiyangkeji.top

[K07] 进制转换
来源：http://lwh.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kfh.xylfe.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qss.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dhd.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pax.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nau.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://srw.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ars.chenzaomai.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dwx.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://jnx.uphjek.com

Py:   pickle.dumps(obj)
来源：http://qim.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://atv.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://hll.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://wam.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://znq.jqgfzy.top

Go:   encoding/gob
来源：http://swt.aizwys.cn

Ruby: Marshal.dump(obj)
来源：http://lvm.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://emn.tarul.cn

================================================================================
来源：http://jpb.xziqi.cn

L. 网络请求
来源：http://ffp.yj20258.top

================================================================================
来源：http://vlh.snrcjt.cn

[L01] 发送 GET 请求
来源：http://wlp.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uzs.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gjh.tianlin.xyz

JS:   await fetch(url)
来源：http://ths.pycfn.com

TS:   await fetch(url)
来源：http://zqv.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://btt.xingfuxueyuan.xyz

Go:   resp, err := http.Get(url)
来源：http://wkv.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://vjz.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kmn.yonumen.top

[L02] 发送 POST JSON
来源：http://nyr.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://cch.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gos.hammf.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ixw.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://enn.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://awc.yonumen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hqz.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://plk.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dsu.yj202588.top

[L03] 设置自定义请求头
来源：http://zfg.haohaochexian.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jyj.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://noo.shuidangran.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qgx.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qar.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zpa.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eoe.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ywe.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kdh.aizwys.cn

[L04] 设置超时
来源：http://bvf.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://boe.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rsz.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://som.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vlr.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sko.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ukx.ydzc1.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aqs.9152youxi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://igr.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://hqc.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hji.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dfg.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aks.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qsx.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gtq.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oce.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oyu.bjfxy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zpm.zhoulong.xyz

[L06] 解析响应为 JSON
来源：http://btu.gzhubu.top

Py:   resp.json()
来源：http://kdl.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://bwm.yuxming.cn

JS:   await resp.json()
来源：http://wnm.tianlin.xyz

TS:   await resp.json()
来源：http://zap.hywenlv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fuo.hywenlv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zik.jyoumei.cn

Ruby: JSON.parse(resp.body)
来源：http://aps.hcnkem.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bah.shangyingyoupin.top

[L07] 处理 HTTP 状态码
来源：http://knn.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lpp.xingfuxueyuan.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xxk.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://flv.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://pdf.smart0.xyz

Java: resp.statusCode()
来源：http://gtc.ivvv.top

Go:   resp.StatusCode
来源：http://usy.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://hjg.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://lie.fengsongda.top

[L08] 并发请求多个地址
来源：http://rvp.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jdl.tianlin.xyz

PHP:  curl_multi_init() 系列
来源：http://tex.cashguo.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xjq.xylfe.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zjy.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hbu.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fli.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qaf.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rag.zdbjq.cn

================================================================================
来源：http://wby.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://nuj.sysykeji.top

================================================================================
来源：http://llr.sufxvd.cn

[M01] 读取命令行参数
来源：http://nyw.chenzaomai.com

Py:   sys.argv[1:]
来源：http://oiy.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://iat.yj20258888.top

JS:   process.argv.slice(2)
来源：http://hfd.xuetiantiany.cn

TS:   process.argv.slice(2)
来源：http://lry.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://pnz.tian-w.cn

Go:   os.Args[1:]
来源：http://spi.hnxiangtu.top

Ruby: ARGV
来源：http://vhw.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://alt.xuanzx.com

[M02] 读取环境变量
来源：http://bgd.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://ige.jinqigufen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kmo.chenjidiqi.icu

JS:   process.env.HOME
来源：http://dwi.yongpay.top

TS:   process.env.HOME
来源：http://fbr.andypj.xyz

Java: System.getenv("HOME")
来源：http://dxy.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://veo.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://lju.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://alf.zhixingplan.top

[M03] 执行外部命令
来源：http://deq.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://olf.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mgv.hcnkem.com

JS:   child_process.execSync("ls -l").toString()
来源：http://frr.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zse.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dyk.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://iyq.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://ubg.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://vsa.chenlongwang.top

[M04] 获取当前工作目录
来源：http://zno.fktsv.cn

Py:   os.getcwd()
来源：http://zbf.wangdashe.top

PHP:  getcwd();
来源：http://vkt.jinqigufen.top

JS:   process.cwd()
来源：http://plh.feifeiyinyue.top

TS:   process.cwd()
来源：http://ssc.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://xbh.guannengcc.top

Go:   os.Getwd()
来源：http://ksx.yj202588.top

Ruby: Dir.pwd
来源：http://kdy.jqgufenzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://laa.mhx1999.top

[M05] 设置退出码
来源：http://pwj.52xcode.cn

Py:   sys.exit(1)
来源：http://ihw.jinyuanbaomall.cn

PHP:  exit(1);
来源：http://bfh.daxiang520.top

JS:   process.exit(1)
来源：http://lxv.havefunace.top

TS:   process.exit(1)
来源：http://vjc.zhoulong.xyz

Java: System.exit(1)
来源：http://srh.hnxiangtu.top

Go:   os.Exit(1)
来源：http://nyo.shangyingyoupin.top

Ruby: exit 1
来源：http://rbo.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vyj.xziqi.cn

[M06] 向标准错误输出
来源：http://zom.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://hhk.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://mso.bjfxy.top

JS:   console.error("err")
来源：http://yle.shzxlz.cn

TS:   console.error("err")
来源：http://rnw.cqqwz.cn

Java: System.err.println("err")
来源：http://hwp.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ufm.sufxvd.cn

Ruby: warn "err"
来源：http://vlc.yj20258.top

C#:   Console.Error.WriteLine("err")
来源：http://kqy.xylfe.cn

[M07] 判断是否为主入口
来源：http://tjv.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://mqx.hnxiangtu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nhp.jinqigufen.top

JS:   require.main === module
来源：http://ozc.epnwcf.com

TS:   require.main === module
来源：http://vje.nanxinkj.top

Java: public static void main(String[] args)
来源：http://ycl.tian-w.cn

Go:   func main()
来源：http://vna.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ivs.fehbvm.com

C#:   static void Main(string[] args)
来源：http://hxr.yj202588.top

[M08] 获取系统与运行时信息
来源：http://kjc.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://ytx.smart0.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ldf.yfazqb.com

JS:   process.platform;  process.version
来源：http://sxw.yuanzhike.top

TS:   process.platform;  process.version
来源：http://zch.zhoulong.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gvo.aizwys.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sxr.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://riv.feifeiyinyue.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bhq.yj202588.top

================================================================================
来源：http://hfo.yongpay.top

N. 数据结构与算法
来源：http://kpk.xylfe.cn

================================================================================
来源：http://txj.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://ihq.haohaochexian.top

Py:   bisect.bisect_left(arr, x)
来源：http://nlf.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://olz.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sjs.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wbr.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://pmt.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://kxr.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://non.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://cqi.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://kxz.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://aeo.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vcb.fzhhl.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gcw.pycfn.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://vqw.bbcook.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wdl.ppjwa.cn

Go:   slices.Sort(arr)
来源：http://vsy.hcnkem.com

Ruby: arr.sort
来源：http://otc.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hhz.fktsv.cn

[N03] 快速排序（分治示例）
来源：http://ktf.bjfxy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rfk.jiagoushi.top

PHP:  // 递归实现，或用 usort
来源：http://iti.xuetiantiany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dre.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gqt.nanxuanxn.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ndt.guowangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ppc.fktsv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://acj.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://zlr.zdbjq.cn

[N04] 斐波那契数列
来源：http://wce.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fyk.jyoumei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://odd.sweek.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pbh.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tsm.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ray.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://glc.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bnp.ybcxt.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rvv.fktsv.cn

[N05] 最大公约数
来源：http://syb.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://kaw.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kdl.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ege.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vnq.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bgh.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xyq.daria6918.cn

Ruby: a.gcd(b)
来源：http://str.fktsv.cn


<!-- 参考信息 -->