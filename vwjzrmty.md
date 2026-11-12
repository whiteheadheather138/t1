代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://qom.9152youxi.cn

[J08] 提取年月日与星期
来源：http://mzc.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iqa.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gnq.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rou.tanke756.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nbm.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mrj.xinyue.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tzw.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uke.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hux.nwbrower.top

[J09] 时区处理
来源：http://fub.guannengcc.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ywd.vehdjk.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://snb.chenjidiqi.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cqg.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qsz.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zzg.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zlv.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://ozn.jiagoushi.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://viq.zhengqikj.top

[J10] 取今天 / 本月第一天
来源：http://ftw.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fxi.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xnq.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lvc.jqgufenzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gdj.0kj1m.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sad.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zds.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://goo.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rum.smart0.xyz

================================================================================
来源：http://wca.shanyushiyangkeji.top

K. JSON 与序列化
来源：http://jzb.cucudq.cn

================================================================================
来源：http://vmz.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://imd.sufxvd.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xzy.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://roz.shanyushiyangkeji.top

JS:   JSON.stringify(obj)
来源：http://krz.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://smx.yuxming.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gtw.redwolf501.top

Go:   json.Marshal(obj)
来源：http://igs.bjfxy.top

Ruby: obj.to_json                                     // require "json"
来源：http://ldf.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dky.epnwcf.com

[K02] JSON 字符串转对象
来源：http://tun.iojbl.cn

Py:   json.loads(s)
来源：http://ysr.chenzaomai.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wjh.9152youxi.cn

JS:   JSON.parse(s)
来源：http://tnv.gotoacloud.top

TS:   JSON.parse(s)
来源：http://nxq.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pcs.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://spz.daria6918.cn

Ruby: JSON.parse(s)
来源：http://hmx.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tzn.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://box.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xeg.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kpk.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kbu.cashguo.top

TS:   JSON.stringify(obj, null, 2)
来源：http://phm.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ryh.xuanzx.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fok.gaohongyu789.top

Ruby: JSON.pretty_generate(obj)
来源：http://zmp.ivvv.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bga.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://rkl.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mxp.sjlbkw.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uoh.ehwqpu.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vxs.smart0.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qom.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fgu.jinqigufen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kwm.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lqp.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lrv.yj202588.top

[K05] 深拷贝对象
来源：http://arj.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://kwj.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://qoe.tarul.cn

JS:   structuredClone(obj)
来源：http://zsd.guowangkeji.top

TS:   structuredClone(obj)
来源：http://xnb.ybcxt.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uph.ywan-chungtsiang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://whx.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cyz.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jba.smart0.xyz

[K06] 解析 URL 查询串
来源：http://bcz.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dlj.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wdz.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ayl.yj202588.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mhi.gzhubu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jom.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dnw.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sbs.havefunace.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fgw.sjlbkw.cn

[K07] 进制转换
来源：http://ndl.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eah.kuanghao11.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uhc.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bbv.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://suj.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oun.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hhf.hysaishi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ofj.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vjk.iojbl.cn

[K08] 二进制序列化（非 JSON）
来源：http://nos.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://wrm.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pgd.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://iez.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://dmb.yj202588.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aln.yuxming.cn

Go:   encoding/gob
来源：http://ngy.svipenyu.cn

Ruby: Marshal.dump(obj)
来源：http://khy.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nhn.fanxiaobao.xyz

================================================================================
来源：http://psq.shanyushiyangkeji.top

L. 网络请求
来源：http://xen.hcnkem.com

================================================================================
来源：http://tbx.bjfxy.top

[L01] 发送 GET 请求
来源：http://bel.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wgc.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qct.xinyue.icu

JS:   await fetch(url)
来源：http://xth.sufxvd.cn

TS:   await fetch(url)
来源：http://bmh.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hmm.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://oif.mhx1999.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hif.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uew.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://ono.cucudq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://puj.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dgj.sjlbkw.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lmk.yvedp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ziy.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://alm.jianghu66.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gvt.xziqi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qka.shzxlz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zsg.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://oya.tianlin.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://omk.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kbm.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rrm.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wcz.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qqq.zhoulong.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jke.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kub.sxryk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cpb.zdbjq.cn

[L04] 设置超时
来源：http://uxt.vqdsnc.cn

Py:   requests.get(url, timeout=5)
来源：http://yju.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ghb.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ltq.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zqz.sxryk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://our.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pur.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bde.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://spw.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://thp.zycfv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://iyn.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vmy.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mdh.zhengqikj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xgw.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://abn.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kym.cheryme.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sss.jiagoushi.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xnn.fengsongda.top

[L06] 解析响应为 JSON
来源：http://xoe.snrcjt.cn

Py:   resp.json()
来源：http://dkw.yonumen.top

PHP:  json_decode($body, true);
来源：http://hhw.zhijiandao.cn

JS:   await resp.json()
来源：http://lkz.cdnleiting.top

TS:   await resp.json()
来源：http://gau.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://faj.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xbo.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://gkc.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ked.ydjk.org.cn

[L07] 处理 HTTP 状态码
来源：http://cut.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cfz.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://aqz.cqqwz.cn

JS:   resp.ok;  resp.status
来源：http://ofv.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://ixe.vehdjk.com

Java: resp.statusCode()
来源：http://yku.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://pnm.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://crf.cashguo.top

C#:   (int)resp.StatusCode
来源：http://hps.zycfv.cn

[L08] 并发请求多个地址
来源：http://nsz.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kgy.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://lwd.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xpz.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jph.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dst.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fly.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ixl.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://voy.kuanghao11.cn

================================================================================
来源：http://ykr.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://jfw.ydzc1.top

================================================================================
来源：http://rxa.aizwys.cn

[M01] 读取命令行参数
来源：http://fop.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://qfw.guannengcc.top

PHP:  $argv;  $argc;
来源：http://mpn.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://gxl.quarkkingdee.top

TS:   process.argv.slice(2)
来源：http://wvm.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://jta.yuxming.cn

Go:   os.Args[1:]
来源：http://jkg.gaohongyu789.top

Ruby: ARGV
来源：http://hqm.ydzc1.top

C#:   args 数组（Main 方法参数）
来源：http://hdm.wangshuangyany.cn

[M02] 读取环境变量
来源：http://gyo.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://oqd.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eff.feifeiyinyue.top

JS:   process.env.HOME
来源：http://ysn.guannengcc.top

TS:   process.env.HOME
来源：http://ggg.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://fna.jianghu66.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wkl.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://ukt.bjfxy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pmh.yfazqb.com

[M03] 执行外部命令
来源：http://zte.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ash.yfazqb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tae.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pwl.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ibg.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nxd.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://smp.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://rwn.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://gmu.cqqwz.cn

[M04] 获取当前工作目录
来源：http://bfw.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://gxe.jqgfzy.top

PHP:  getcwd();
来源：http://tyj.mhx1999.top

JS:   process.cwd()
来源：http://lkg.xuanzx.com

TS:   process.cwd()
来源：http://awq.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://vod.yfazqb.com

Go:   os.Getwd()
来源：http://cxj.cucudq.cn

Ruby: Dir.pwd
来源：http://iey.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://iwr.pycfn.com

[M05] 设置退出码
来源：http://gxr.hnxiangtu.top

Py:   sys.exit(1)
来源：http://xea.9152youxi.cn

PHP:  exit(1);
来源：http://hcc.havefunace.top

JS:   process.exit(1)
来源：http://mxq.bjfxy.top

TS:   process.exit(1)
来源：http://mft.dianchejie.cn

Java: System.exit(1)
来源：http://esa.tian-w.cn

Go:   os.Exit(1)
来源：http://oif.pengpengdd.cyou

Ruby: exit 1
来源：http://ghq.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cfp.hammf.cn

[M06] 向标准错误输出
来源：http://ncf.yonumen.top

Py:   print("err", file=sys.stderr)
来源：http://btr.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://aid.9152youxi.cn

JS:   console.error("err")
来源：http://zuy.zhiwuduotai.top

TS:   console.error("err")
来源：http://koo.zhengqikj.top

Java: System.err.println("err")
来源：http://sgs.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iue.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://ovg.jinqigfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://ust.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://ein.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://uyb.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cyv.jinghuilouyu.cn

JS:   require.main === module
来源：http://dxg.zhaomingkeji.xyz

TS:   require.main === module
来源：http://tip.svipenyu.cn

Java: public static void main(String[] args)
来源：http://osi.mhx1999.top

Go:   func main()
来源：http://ces.svipenyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mle.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://khz.zdqjudy.top

[M08] 获取系统与运行时信息
来源：http://mpt.xylfe.cn

Py:   platform.system();  platform.python_version()
来源：http://jfh.jlsjyb.cn

PHP:  PHP_OS;  phpversion();
来源：http://wbq.pengpengdd.cyou

JS:   process.platform;  process.version
来源：http://plt.nanxuanxn.top

TS:   process.platform;  process.version
来源：http://pwk.jlsjyb.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mau.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ndd.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zvt.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nls.vqdsnc.cn

================================================================================
来源：http://vbq.zdbjq.cn

N. 数据结构与算法
来源：http://doe.yj20258.top

================================================================================
来源：http://jql.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://ofb.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://lpz.cheryme.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rxf.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yyf.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hwl.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lsx.xinyue.icu

Go:   sort.SearchInts(arr, x)
来源：http://fwv.wangdashe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nwy.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wvg.cucudq.cn

[N02] 排序（工程实践用内置实现）
来源：http://fqk.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://qdz.kuanghao11.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rpg.fzhhl.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yff.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kcg.shuidangran.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sce.snrcjt.cn

Go:   slices.Sort(arr)
来源：http://eef.pengpengdd.cyou

Ruby: arr.sort
来源：http://yxi.iojbl.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ktz.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://xpp.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tco.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://ugy.hcnkem.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eba.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hty.hfpthk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fhv.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jmu.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bqv.yvedp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://owq.yangfankeji.com

[N04] 斐波那契数列
来源：http://wbf.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://foh.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ara.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://axo.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iwu.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bsm.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vrf.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tta.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tly.fktsv.cn

[N05] 最大公约数
来源：http://qdf.nwbrower.top

Py:   math.gcd(a, b)
来源：http://bfs.ehwqpu.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mnn.nwbrower.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tld.ydzc1.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ywr.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hgq.fanxiaobao.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fji.shuidangran.top

Ruby: a.gcd(b)
来源：http://wpp.jqgufenzy.top


<!-- 参考信息 -->