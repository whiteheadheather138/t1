代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://nvs.yanxiufei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pft.cheryme.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lof.epnwcf.com

Ruby: d1 < d2;  d1 == d2
来源：http://etq.yfazqb.com

C#:   d1 < d2;  d1 == d2
来源：http://pgk.gogol.net.cn

[J08] 提取年月日与星期
来源：http://csg.hywenlv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tzx.yj20258.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jtb.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bez.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ozo.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sft.havefunace.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jji.aizwys.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jjo.redwolf501.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gym.jqgfzy.top

[J09] 时区处理
来源：http://vzm.chenjidiqi.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://odw.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zlo.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bir.zdbjq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://joo.wangdashe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dku.hnxiangtu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dew.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rto.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ewu.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://jkp.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://owf.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mkn.haohaochexian.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fno.zhijiandao.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kev.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ohv.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qvk.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rbt.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ipc.haohaochexian.top

================================================================================
来源：http://vra.cqqwz.cn

K. JSON 与序列化
来源：http://les.yvedp.cn

================================================================================
来源：http://hzf.epnwcf.com

[K01] 对象转 JSON 字符串
来源：http://peq.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tbu.dashuyun.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qvq.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://dlu.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://zdl.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gvq.yonumen.top

Go:   json.Marshal(obj)
来源：http://zpd.uphjek.com

Ruby: obj.to_json                                     // require "json"
来源：http://fbn.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cwy.aibaodan.cn

[K02] JSON 字符串转对象
来源：http://ciy.9152youxi.cn

Py:   json.loads(s)
来源：http://vce.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://voy.chenzaomai.com

JS:   JSON.parse(s)
来源：http://dns.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://bxb.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wzg.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://ckt.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://zif.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vty.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://bsa.sysykeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nck.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://muo.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://mzo.ehwqpu.com

TS:   JSON.stringify(obj, null, 2)
来源：http://swv.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xuw.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rqf.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://lhg.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bjm.xuanzx.com

[K04] 读取 JSON 文件
来源：http://xvo.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gaj.pycfn.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tsx.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eev.bjfxy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qdx.dashuyun.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://axb.havefunace.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zll.nwbrower.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://utt.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xkf.0kj1m.cn

[K05] 深拷贝对象
来源：http://yay.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://rcj.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://xit.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://jqy.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://olu.xinyue.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://kox.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vfi.jiagoushi.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tpz.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ghu.ivvv.top

[K06] 解析 URL 查询串
来源：http://ert.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rky.nanxuanxn.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vsl.daxiang520.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://opa.tianlin.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ujj.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pcn.wangshuangyany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://frc.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qpu.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dbv.nwbrower.top

[K07] 进制转换
来源：http://wmf.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lko.zycfv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bla.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://che.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sbp.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jha.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://huz.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qzf.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cii.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://sel.nwbrower.top

Py:   pickle.dumps(obj)
来源：http://jfg.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sfw.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://boa.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://fbf.ydjk.org.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dlc.xinyue.icu

Go:   encoding/gob
来源：http://rmw.fengsongda.top

Ruby: Marshal.dump(obj)
来源：http://uwi.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://acv.yvedp.cn

================================================================================
来源：http://job.vqdsnc.cn

L. 网络请求
来源：http://zst.c1oappe.top

================================================================================
来源：http://enp.guannengcc.top

[L01] 发送 GET 请求
来源：http://smt.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nmk.0kj1m.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rgm.xuetiantiany.cn

JS:   await fetch(url)
来源：http://pac.iojbl.cn

TS:   await fetch(url)
来源：http://svg.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://awc.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://dld.feifeiyinyue.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zre.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hck.snrcjt.cn

[L02] 发送 POST JSON
来源：http://nbg.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qtd.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nkh.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qvv.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bqz.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lio.jinyuanbaomall.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ypt.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ext.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ciq.cqqwz.cn

[L03] 设置自定义请求头
来源：http://ivn.jyoumei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nlw.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mqd.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dgl.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kud.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qew.gzhubu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rly.daxiang520.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qdy.shuidangran.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nfv.hnxiangtu.top

[L04] 设置超时
来源：http://eaq.vehdjk.com

Py:   requests.get(url, timeout=5)
来源：http://fge.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hby.bbcook.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kks.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://brt.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jqg.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ldp.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://krk.havefunace.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jxc.mhx1999.top

[L05] 上传文件（multipart）
来源：http://nht.epnwcf.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wli.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://seo.cdnleiting.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uzo.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hvu.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hxt.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gfm.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ugq.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kys.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://okc.nanxuanxn.top

Py:   resp.json()
来源：http://vth.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://msj.gogol.net.cn

JS:   await resp.json()
来源：http://doh.ctjpmb.com

TS:   await resp.json()
来源：http://tkr.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mqy.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ijy.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://yfd.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cod.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://rdo.sweek.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mhe.snrcjt.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ngk.xingfuxueyuan.xyz

JS:   resp.ok;  resp.status
来源：http://ycc.zhengqikj.top

TS:   resp.ok;  resp.status
来源：http://ncb.yj20258.top

Java: resp.statusCode()
来源：http://fdn.aizwys.cn

Go:   resp.StatusCode
来源：http://etl.shanyushiyangkeji.top

Ruby: resp.code.to_i
来源：http://zre.xuetiantiany.cn

C#:   (int)resp.StatusCode
来源：http://ska.jinqigufen.top

[L08] 并发请求多个地址
来源：http://fdc.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uhz.kuanghao11.cn

PHP:  curl_multi_init() 系列
来源：http://wso.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sny.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wuz.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vlg.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sdi.jlsjyb.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ezh.hysaishi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hut.yuanzhike.top

================================================================================
来源：http://epi.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://mbp.hnxiangtu.top

================================================================================
来源：http://chb.hongshengwenyu.top

[M01] 读取命令行参数
来源：http://kht.jinqigfzy.top

Py:   sys.argv[1:]
来源：http://gjz.cucudq.cn

PHP:  $argv;  $argc;
来源：http://gil.ydjk.org.cn

JS:   process.argv.slice(2)
来源：http://wyy.guannengcc.top

TS:   process.argv.slice(2)
来源：http://zhi.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://hys.uphjek.com

Go:   os.Args[1:]
来源：http://nhl.ivvv.top

Ruby: ARGV
来源：http://gym.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://uhu.tianlin.xyz

[M02] 读取环境变量
来源：http://rwz.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://zky.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vce.ppjwa.cn

JS:   process.env.HOME
来源：http://knh.birdmap.top

TS:   process.env.HOME
来源：http://pqw.yonumen.top

Java: System.getenv("HOME")
来源：http://trg.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://drm.hammf.cn

Ruby: ENV["HOME"]
来源：http://sfs.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vxt.sysykeji.top

[M03] 执行外部命令
来源：http://ynt.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xec.yvedp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zhk.vehdjk.com

JS:   child_process.execSync("ls -l").toString()
来源：http://yku.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://olj.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://omf.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://smp.yanxiufei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://csn.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://npl.birdmap.top

[M04] 获取当前工作目录
来源：http://zjo.chenjidiqi.icu

Py:   os.getcwd()
来源：http://aim.316326.xyz

PHP:  getcwd();
来源：http://aqn.chenzaomai.com

JS:   process.cwd()
来源：http://fdu.uphjek.com

TS:   process.cwd()
来源：http://uhf.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://ddv.316326.xyz

Go:   os.Getwd()
来源：http://vlo.sweek.top

Ruby: Dir.pwd
来源：http://cfz.sjlbkw.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nli.yj20258888.top

[M05] 设置退出码
来源：http://uck.xingfuxueyuan.xyz

Py:   sys.exit(1)
来源：http://tes.hcnkem.com

PHP:  exit(1);
来源：http://kfz.uphjek.com

JS:   process.exit(1)
来源：http://csw.hywenlv.cn

TS:   process.exit(1)
来源：http://sgd.hysaishi.cn

Java: System.exit(1)
来源：http://yig.ppjwa.cn

Go:   os.Exit(1)
来源：http://ecb.pycfn.com

Ruby: exit 1
来源：http://rho.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nfr.dianchejie.cn

[M06] 向标准错误输出
来源：http://qnn.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://evl.52xcode.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wlh.zhongyouzk.top

JS:   console.error("err")
来源：http://xmf.chenlongwang.top

TS:   console.error("err")
来源：http://ctg.fehbvm.com

Java: System.err.println("err")
来源：http://iyd.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://znz.dashuyun.cn

Ruby: warn "err"
来源：http://bkb.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://gzy.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://kee.jinqigufen.top

Py:   if __name__ == "__main__":
来源：http://xes.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ybz.jinghuilouyu.cn

JS:   require.main === module
来源：http://mmx.redwolf501.top

TS:   require.main === module
来源：http://ttx.jiagoushi.top

Java: public static void main(String[] args)
来源：http://otn.xylfe.cn

Go:   func main()
来源：http://edt.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://clv.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://pww.fzhhl.top

[M08] 获取系统与运行时信息
来源：http://idr.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://fqg.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://ovg.yuanzhike.top

JS:   process.platform;  process.version
来源：http://pjd.haohaochexian.top

TS:   process.platform;  process.version
来源：http://hsg.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ptf.ppjwa.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xgh.zhiwuduotai.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hur.wangshuangyany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://poy.kuanghao11.cn

================================================================================
来源：http://cpz.uphjek.com

N. 数据结构与算法
来源：http://gex.fehbvm.com

================================================================================
来源：http://yzt.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://qjj.zhiwuduotai.top

Py:   bisect.bisect_left(arr, x)
来源：http://izp.jianghu66.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://asv.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ubv.chenlongwang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pvn.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://cdn.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://rxz.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vbg.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kdh.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://eut.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://ctg.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gpl.yueranfly.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tux.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://axk.tanke756.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cps.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://mdh.tarul.cn

Ruby: arr.sort
来源：http://zvi.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://moz.yangfankeji.com

[N03] 快速排序（分治示例）
来源：http://xja.ppjwa.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zwx.jiagoushi.top

PHP:  // 递归实现，或用 usort
来源：http://sgv.sysykeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jtw.shzxlz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mua.yj202588.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ckr.yuanzhike.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ktk.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nyq.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oad.bjfxy.top

[N04] 斐波那契数列
来源：http://usg.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://unh.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://btv.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://exf.jinqigufen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://opr.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://edj.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zvn.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yox.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gby.daria6918.cn

[N05] 最大公约数
来源：http://xgb.fktsv.cn

Py:   math.gcd(a, b)
来源：http://cej.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vms.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gdp.ivvv.top


<!-- 参考信息 -->