代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://jsk.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pvu.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eyj.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://bps.iojbl.cn

C#:   d1 < d2;  d1 == d2
来源：http://xro.hammf.cn

[J08] 提取年月日与星期
来源：http://ryk.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://swg.yongpay.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mos.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rag.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yjz.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fyw.xylfe.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://noh.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pqc.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qnd.ywan-chungtsiang.top

[J09] 时区处理
来源：http://pba.guannengcc.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xjr.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ivl.fanxiaobao.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zjz.wangshuangyany.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sbn.sxryk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hjw.wangdashe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gzl.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ken.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hhk.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://dda.vqdsnc.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hob.fengsongda.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fls.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://itq.hnqzz.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lxq.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mwa.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ulj.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yda.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://exn.gotoacloud.top

================================================================================
来源：http://tze.yangfankeji.com

K. JSON 与序列化
来源：http://oey.haohaochexian.top

================================================================================
来源：http://rzy.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://vca.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lue.jqgfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nny.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://qah.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://aoo.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rru.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://dvm.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://vke.tanke756.top

C#:   JsonSerializer.Serialize(obj)
来源：http://srq.vehdjk.com

[K02] JSON 字符串转对象
来源：http://fnp.tian-w.cn

Py:   json.loads(s)
来源：http://bpn.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ftj.daria6918.cn

JS:   JSON.parse(s)
来源：http://rdp.andypj.xyz

TS:   JSON.parse(s)
来源：http://hbt.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ovb.zycfv.cn

Go:   json.Unmarshal(data, &v)
来源：http://bon.yueranfly.top

Ruby: JSON.parse(s)
来源：http://nqd.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aqg.vehdjk.com

[K03] JSON 美化输出（带缩进）
来源：http://cnq.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xff.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mcl.daria6918.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://buh.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jzi.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qxc.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hkw.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://fql.epnwcf.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gna.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://weu.jianghu66.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qse.yangfankeji.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tbi.bjfxy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://acj.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xny.hywenlv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aux.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fly.redwolf501.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tpy.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xwe.zhiwuduotai.top

[K05] 深拷贝对象
来源：http://vwv.sysykeji.top

Py:   copy.deepcopy(obj)
来源：http://mey.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://jts.hcnkem.com

JS:   structuredClone(obj)
来源：http://wuj.yangfankeji.com

TS:   structuredClone(obj)
来源：http://kib.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://txx.yuxming.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eoj.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bxn.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://foe.bbcook.cn

[K06] 解析 URL 查询串
来源：http://hcg.fzhhl.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ylj.vqdsnc.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oic.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dbg.chenlongwang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cxs.hongshengwenyu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sqj.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://xee.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cth.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zxh.hcnkem.com

[K07] 进制转换
来源：http://xzd.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wyw.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qwq.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vvh.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rqa.yanxiufei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wqq.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ozb.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lku.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dfu.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://azw.cheryme.top

Py:   pickle.dumps(obj)
来源：http://tpg.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ekx.jqgfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://qyn.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://wks.yonumen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nyc.yangfankeji.com

Go:   encoding/gob
来源：http://vyy.aizwys.cn

Ruby: Marshal.dump(obj)
来源：http://uvv.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lyp.zhijiandao.cn

================================================================================
来源：http://hzx.zhiwuduotai.top

L. 网络请求
来源：http://vcd.nanxinkj.top

================================================================================
来源：http://pzd.ivvv.top

[L01] 发送 GET 请求
来源：http://kng.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ljp.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ysi.vehdjk.com

JS:   await fetch(url)
来源：http://ien.tanke756.top

TS:   await fetch(url)
来源：http://sap.nwbrower.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xrn.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://tag.ivvv.top

Ruby: Net::HTTP.get(URI(url))
来源：http://okv.jinyuanbaomall.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dbb.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://fpc.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://xhr.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pzk.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wnl.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eza.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iee.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mcj.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gus.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dmo.ydjk.org.cn

[L03] 设置自定义请求头
来源：http://apt.yj20258888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gtg.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ydh.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://haj.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ylj.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gno.chenzaomai.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fcc.tanke756.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sns.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ibm.yongpay.top

[L04] 设置超时
来源：http://quf.zdqjudy.top

Py:   requests.get(url, timeout=5)
来源：http://prg.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dyw.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rnv.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gwc.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zfx.epnwcf.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jeg.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mql.ehwqpu.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yxw.c1oappe.top

[L05] 上传文件（multipart）
来源：http://fxd.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yvv.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yro.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://omz.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wnh.zdbjq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://njj.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cds.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kua.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nob.316326.xyz

[L06] 解析响应为 JSON
来源：http://yke.snrcjt.cn

Py:   resp.json()
来源：http://bzj.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://wpl.snrcjt.cn

JS:   await resp.json()
来源：http://oer.ydjk.org.cn

TS:   await resp.json()
来源：http://viy.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sco.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jhj.zhiwuduotai.top

Ruby: JSON.parse(resp.body)
来源：http://ksr.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://asz.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://pnx.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qsq.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rvi.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://dqb.xingfuxueyuan.xyz

TS:   resp.ok;  resp.status
来源：http://jvk.hammf.cn

Java: resp.statusCode()
来源：http://hae.fzhhl.top

Go:   resp.StatusCode
来源：http://nug.guowangkeji.top

Ruby: resp.code.to_i
来源：http://qks.tanke756.top

C#:   (int)resp.StatusCode
来源：http://uja.yongpay.top

[L08] 并发请求多个地址
来源：http://hfc.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kxa.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://uwl.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rbo.zdbjq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kjc.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wwk.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zpk.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ecr.aizwys.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ttp.daria6918.cn

================================================================================
来源：http://snm.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://sju.c1oappe.top

================================================================================
来源：http://aei.bjfxy.top

[M01] 读取命令行参数
来源：http://fsg.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://dvo.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://mbh.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://vmo.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://hbi.cqqwz.cn

Java: args 数组（main 方法参数）
来源：http://lus.ctjpmb.com

Go:   os.Args[1:]
来源：http://sdm.zhoulong.xyz

Ruby: ARGV
来源：http://pjq.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://jcm.sufxvd.cn

[M02] 读取环境变量
来源：http://eqd.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://nwl.hammf.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nns.gotoacloud.top

JS:   process.env.HOME
来源：http://sim.zhiwuduotai.top

TS:   process.env.HOME
来源：http://kir.fehbvm.com

Java: System.getenv("HOME")
来源：http://etm.hesvh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://owb.hcnkem.com

Ruby: ENV["HOME"]
来源：http://wqw.ydjk.org.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dds.9152youxi.cn

[M03] 执行外部命令
来源：http://uaw.bbcook.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rej.yanxiufei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dms.sxryk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hce.316326.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://qpq.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rwr.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://phq.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://fte.jinqigufen.top

C#:   Process.Start("ls", "-l");
来源：http://hhe.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://bpe.dianchejie.cn

Py:   os.getcwd()
来源：http://jkp.jlsjyb.cn

PHP:  getcwd();
来源：http://tie.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://kpu.havefunace.top

TS:   process.cwd()
来源：http://hlg.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://kvj.svipenyu.cn

Go:   os.Getwd()
来源：http://sut.shanyushiyangkeji.top

Ruby: Dir.pwd
来源：http://afv.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://cle.cdnleiting.top

[M05] 设置退出码
来源：http://sis.xuanzx.com

Py:   sys.exit(1)
来源：http://vky.meibo888.top

PHP:  exit(1);
来源：http://kgn.cashguo.top

JS:   process.exit(1)
来源：http://hbu.hnqzz.top

TS:   process.exit(1)
来源：http://xry.zycfv.cn

Java: System.exit(1)
来源：http://uyz.jinyuanbaomall.cn

Go:   os.Exit(1)
来源：http://til.kuanghao11.cn

Ruby: exit 1
来源：http://nxv.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ynr.yuanzhike.top

[M06] 向标准错误输出
来源：http://gtv.fehbvm.com

Py:   print("err", file=sys.stderr)
来源：http://oqq.hfpthk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bvm.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://jto.birdmap.top

TS:   console.error("err")
来源：http://daa.jianghu66.top

Java: System.err.println("err")
来源：http://gqy.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yff.tanke756.top

Ruby: warn "err"
来源：http://euu.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://qsu.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://axg.cashguo.top

Py:   if __name__ == "__main__":
来源：http://fri.zhiwuduotai.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xmk.tianlin.xyz

JS:   require.main === module
来源：http://qps.smart0.xyz

TS:   require.main === module
来源：http://bim.cucudq.cn

Java: public static void main(String[] args)
来源：http://soy.ppjwa.cn

Go:   func main()
来源：http://bgu.guowangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://seo.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://kun.yj20258.top

[M08] 获取系统与运行时信息
来源：http://xkd.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://yrq.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://bul.ehwqpu.com

JS:   process.platform;  process.version
来源：http://gre.daria6918.cn

TS:   process.platform;  process.version
来源：http://tvk.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://azy.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://par.fengsongda.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tqu.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hqu.svipenyu.cn

================================================================================
来源：http://xzr.yj20258888.top

N. 数据结构与算法
来源：http://jil.mhx1999.top

================================================================================
来源：http://iwo.sxryk.cn

[N01] 二分查找（有序数组）
来源：http://pnc.fehbvm.com

Py:   bisect.bisect_left(arr, x)
来源：http://ktz.hesvh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qby.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uzb.nanxinkj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jvp.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://phx.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://beb.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nrz.wangshuangyany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://muz.tianlin.xyz

[N02] 排序（工程实践用内置实现）
来源：http://ngj.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://fms.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wkl.zdqjudy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wme.52xcode.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oxo.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mfu.hnxiangtu.top

Go:   slices.Sort(arr)
来源：http://ktp.fktsv.cn

Ruby: arr.sort
来源：http://xoi.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://knj.yj20258.top

[N03] 快速排序（分治示例）
来源：http://qrx.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bok.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://sok.bbcook.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pjc.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ofr.sweek.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zhw.ydzc1.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hkm.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rdb.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://khq.andypj.xyz

[N04] 斐波那契数列
来源：http://yxh.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gqd.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qyf.vqdsnc.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://peb.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ntv.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sie.ivvv.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xqw.gaohongyu789.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hac.iojbl.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jcj.316326.xyz

[N05] 最大公约数
来源：http://nti.yonumen.top

Py:   math.gcd(a, b)
来源：http://csh.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ibv.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mfd.tanke756.top


<!-- 参考信息 -->