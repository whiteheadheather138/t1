代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://cds.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cwb.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hhn.uphjek.com

Ruby: d1 < d2;  d1 == d2
来源：http://kjo.aizwys.cn

C#:   d1 < d2;  d1 == d2
来源：http://caw.jinqigufen.top

[J08] 提取年月日与星期
来源：http://ejc.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lzn.chenlongwang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vbd.ppjwa.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://imo.ehwqpu.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ejp.gzhubu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://htc.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ejp.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mxb.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mdl.cqqwz.cn

[J09] 时区处理
来源：http://wxf.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jtw.zdbjq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qof.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hqe.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://axg.daxiang520.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mri.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jpd.gzhubu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ifb.dianchejie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ghv.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://hzr.hnxiangtu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kgs.jiagoushi.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eoe.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fwr.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iew.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dvo.cdnleiting.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rvj.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xhy.andypj.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vsy.sweek.top

================================================================================
来源：http://jps.zhijiandao.cn

K. JSON 与序列化
来源：http://rti.sysykeji.top

================================================================================
来源：http://asl.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://whl.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oou.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lmc.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://uql.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://npm.guowangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wgt.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://jlb.yfazqb.com

Ruby: obj.to_json                                     // require "json"
来源：http://jwr.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://zcs.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://mtq.hcnkem.com

Py:   json.loads(s)
来源：http://niz.chenjidiqi.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wse.yj202588.top

JS:   JSON.parse(s)
来源：http://ini.iojbl.cn

TS:   JSON.parse(s)
来源：http://wee.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dba.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://abe.yj20258888.top

Ruby: JSON.parse(s)
来源：http://iua.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sqa.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://yud.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tkt.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://czj.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jky.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ysi.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dbm.bjfxy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bzj.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://wey.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nqn.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://fkb.jqgufenzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hnv.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uul.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://azx.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hiv.yuanzhike.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ujs.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cxq.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lsu.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://loi.yueranfly.top

[K05] 深拷贝对象
来源：http://rth.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://bnr.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://iim.zhijiandao.cn

JS:   structuredClone(obj)
来源：http://mwv.tianlin.xyz

TS:   structuredClone(obj)
来源：http://myf.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wjs.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vvm.yongpay.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://chn.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://drd.jinqigfzy.top

[K06] 解析 URL 查询串
来源：http://obv.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lpk.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zwd.ydjk.org.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vrj.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jsl.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rdo.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lum.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ruz.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vms.yanxiufei.cn

[K07] 进制转换
来源：http://ogq.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://loe.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ibe.hywenlv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nkv.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://luo.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fkc.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gld.shzxlz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fbb.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lfu.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://cij.shuidangran.top

Py:   pickle.dumps(obj)
来源：http://wtz.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://hpd.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://wvg.0kj1m.cn

TS:   v8.serialize(obj)        // Node
来源：http://mnv.ivvv.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bkr.hysaishi.cn

Go:   encoding/gob
来源：http://rob.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://ogz.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://obi.zdbjq.cn

================================================================================
来源：http://grs.zhengqikj.top

L. 网络请求
来源：http://ioh.daria6918.cn

================================================================================
来源：http://bjd.zycfv.cn

[L01] 发送 GET 请求
来源：http://uze.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jqk.zhixingplan.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nlw.ybcxt.top

JS:   await fetch(url)
来源：http://wxb.fengsongda.top

TS:   await fetch(url)
来源：http://byj.hammf.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nse.hfpthk.cn

Go:   resp, err := http.Get(url)
来源：http://qkv.tarul.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://scf.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oph.iojbl.cn

[L02] 发送 POST JSON
来源：http://zuc.xylfe.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rmf.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fiv.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gbw.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fmn.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://frk.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jzq.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jak.fzhhl.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://teu.sweek.top

[L03] 设置自定义请求头
来源：http://qtq.chenzaomai.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gqi.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fbl.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tgn.zdqjudy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rvk.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sei.gzhubu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://upq.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://izo.andypj.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://web.cheryme.top

[L04] 设置超时
来源：http://lra.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://hpp.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://svw.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ynl.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kqk.aibaodan.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wkz.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://shn.haohaochexian.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nvw.pengpengdd.cyou

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://szc.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://irk.yfazqb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ehb.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://psf.birdmap.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bqc.52xcode.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sab.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pcr.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qll.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rju.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://npp.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://cig.bbcook.cn

Py:   resp.json()
来源：http://uso.cucudq.cn

PHP:  json_decode($body, true);
来源：http://dcc.birdmap.top

JS:   await resp.json()
来源：http://qav.zdqjudy.top

TS:   await resp.json()
来源：http://twm.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hhu.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qck.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://hpz.iojbl.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ftc.aizwys.cn

[L07] 处理 HTTP 状态码
来源：http://rxd.ppjwa.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nmq.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://amo.hcnkem.com

JS:   resp.ok;  resp.status
来源：http://xou.bbcook.cn

TS:   resp.ok;  resp.status
来源：http://unf.jqgufenzy.top

Java: resp.statusCode()
来源：http://xpl.aizwys.cn

Go:   resp.StatusCode
来源：http://eph.yangfankeji.com

Ruby: resp.code.to_i
来源：http://yav.sjlbkw.cn

C#:   (int)resp.StatusCode
来源：http://fmx.sjlbkw.cn

[L08] 并发请求多个地址
来源：http://yhb.sxryk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jom.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://cxd.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kmf.zycfv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rzs.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ome.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lve.wangdashe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pfa.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://naf.316326.xyz

================================================================================
来源：http://spf.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://vgz.jqgufenzy.top

================================================================================
来源：http://imz.jiagoushi.top

[M01] 读取命令行参数
来源：http://gxw.ybcxt.top

Py:   sys.argv[1:]
来源：http://ysd.cashguo.top

PHP:  $argv;  $argc;
来源：http://nad.yonumen.top

JS:   process.argv.slice(2)
来源：http://hvd.0kj1m.cn

TS:   process.argv.slice(2)
来源：http://eok.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://opg.hywenlv.cn

Go:   os.Args[1:]
来源：http://ipa.hysaishi.cn

Ruby: ARGV
来源：http://orx.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://mjx.pengpengdd.cyou

[M02] 读取环境变量
来源：http://vkn.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://urg.zhongyouzk.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jfx.zhoulong.xyz

JS:   process.env.HOME
来源：http://xfa.nwbrower.top

TS:   process.env.HOME
来源：http://sel.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://ggz.jinqigufen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://erg.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://zzb.xuetiantiany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nhb.gaohongyu789.top

[M03] 执行外部命令
来源：http://faw.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rnc.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kte.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ltw.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://wgd.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ysq.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tuq.yj20258888.top

Ruby: system("ls -l");  `ls -l`
来源：http://akq.ydjk.org.cn

C#:   Process.Start("ls", "-l");
来源：http://jlu.yangfankeji.com

[M04] 获取当前工作目录
来源：http://kqs.c1oappe.top

Py:   os.getcwd()
来源：http://klk.zhixingplan.top

PHP:  getcwd();
来源：http://zlm.52xcode.cn

JS:   process.cwd()
来源：http://ntm.xinyue.icu

TS:   process.cwd()
来源：http://qmx.nwbrower.top

Java: Path.of("").toAbsolutePath()
来源：http://dvg.fktsv.cn

Go:   os.Getwd()
来源：http://ytz.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://saq.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://dwk.52xcode.cn

[M05] 设置退出码
来源：http://xlw.ppjwa.cn

Py:   sys.exit(1)
来源：http://xrb.xinyue.icu

PHP:  exit(1);
来源：http://orl.cheryme.top

JS:   process.exit(1)
来源：http://qfk.fehbvm.com

TS:   process.exit(1)
来源：http://sbu.yj20258888.top

Java: System.exit(1)
来源：http://ybw.guannengcc.top

Go:   os.Exit(1)
来源：http://msf.zhoulong.xyz

Ruby: exit 1
来源：http://rod.zdbjq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fhk.zhijiandao.cn

[M06] 向标准错误输出
来源：http://pyn.guowangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://oci.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://gnb.gzhubu.top

JS:   console.error("err")
来源：http://upa.pengpengdd.cyou

TS:   console.error("err")
来源：http://cvg.iojbl.cn

Java: System.err.println("err")
来源：http://owe.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cue.xinyue.icu

Ruby: warn "err"
来源：http://etp.pycfn.com

C#:   Console.Error.WriteLine("err")
来源：http://fzi.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://kbg.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://oxh.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uhy.ywan-chungtsiang.top

JS:   require.main === module
来源：http://rmm.havefunace.top

TS:   require.main === module
来源：http://fkv.zdqjudy.top

Java: public static void main(String[] args)
来源：http://zkq.yonumen.top

Go:   func main()
来源：http://qnx.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fgf.bjfxy.top

C#:   static void Main(string[] args)
来源：http://wvm.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://lic.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://jgq.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://xme.tanke756.top

JS:   process.platform;  process.version
来源：http://hnw.birdmap.top

TS:   process.platform;  process.version
来源：http://wdt.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jhz.quarkkingdee.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sug.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uob.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zpf.andypj.xyz

================================================================================
来源：http://keh.jqgfzy.top

N. 数据结构与算法
来源：http://tnp.vehdjk.com

================================================================================
来源：http://tia.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://kqp.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://deq.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rtd.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wnz.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xay.52xcode.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mzo.havefunace.top

Go:   sort.SearchInts(arr, x)
来源：http://fai.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qsc.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://zne.havefunace.top

[N02] 排序（工程实践用内置实现）
来源：http://ogr.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://ewg.hysaishi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://icu.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://afp.sjlbkw.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xyh.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cea.bbcook.cn

Go:   slices.Sort(arr)
来源：http://hsc.yangfankeji.com

Ruby: arr.sort
来源：http://tla.nanxuanxn.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gpu.havefunace.top

[N03] 快速排序（分治示例）
来源：http://pef.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://phg.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://omb.cqqwz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://whp.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nqf.andypj.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ezg.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://owd.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ngl.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mts.bjfxy.top

[N04] 斐波那契数列
来源：http://nbw.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gps.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rbk.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dkm.cheryme.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wdo.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://byr.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ytn.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zvg.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://riu.havefunace.top

[N05] 最大公约数
来源：http://ujv.ivvv.top

Py:   math.gcd(a, b)
来源：http://cgg.yongpay.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://taf.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xdk.gogol.net.cn


<!-- 参考信息 -->