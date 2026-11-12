代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://kgc.gotoacloud.top

[J08] 提取年月日与星期
来源：http://vaz.316326.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hpm.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://szf.9152youxi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kla.shanyushiyangtech.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vrk.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uuu.uphjek.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xwe.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tkk.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ynn.jinyuanbaomall.cn

[J09] 时区处理
来源：http://taa.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zzi.tarul.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nky.nanxinkj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nfa.cheryme.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bfy.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zwh.9152youxi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://txm.jinyuanbaomall.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bpr.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ucp.dianchejie.cn

[J10] 取今天 / 本月第一天
来源：http://mmd.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mxs.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wyq.sufxvd.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wtc.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fhf.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ikm.andypj.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://njl.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ury.jinghuilouyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eqs.birdmap.top

================================================================================
来源：http://zap.hysaishi.cn

K. JSON 与序列化
来源：http://qku.zhengqikj.top

================================================================================
来源：http://rij.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://plp.316326.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wam.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ghq.xingfuxueyuan.xyz

JS:   JSON.stringify(obj)
来源：http://wqs.shangyingyoupin.top

TS:   JSON.stringify(obj)
来源：http://pfq.wangshuangyany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mbp.zycfv.cn

Go:   json.Marshal(obj)
来源：http://qmc.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://vkw.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rnq.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://tao.hesvh.cn

Py:   json.loads(s)
来源：http://yww.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gzv.fktsv.cn

JS:   JSON.parse(s)
来源：http://tcf.9152youxi.cn

TS:   JSON.parse(s)
来源：http://ovy.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wqj.bbcook.cn

Go:   json.Unmarshal(data, &v)
来源：http://bpa.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://aps.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lsh.hesvh.cn

[K03] JSON 美化输出（带缩进）
来源：http://xyy.fehbvm.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nbg.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://icf.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://chm.xziqi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mhm.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://awz.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://svh.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://khl.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xbf.kuanghao11.cn

[K04] 读取 JSON 文件
来源：http://rbu.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ffr.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mgj.epnwcf.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://keh.jqgfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ptx.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eak.yueranfly.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ntn.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://lzo.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eja.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://esb.havefunace.top

Py:   copy.deepcopy(obj)
来源：http://nqc.hysaishi.cn

PHP:  unserialize(serialize($obj));
来源：http://krq.xinyue.icu

JS:   structuredClone(obj)
来源：http://cfj.nwbrower.top

TS:   structuredClone(obj)
来源：http://sfk.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bdj.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jrl.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rhb.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://jvu.xylfe.cn

[K06] 解析 URL 查询串
来源：http://jnj.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vfx.quarkkingdee.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wiw.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://otf.ppjwa.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gsd.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cvi.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dga.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ozw.yj202588.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gxz.shanyushiyangtech.top

[K07] 进制转换
来源：http://jtl.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iqx.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qdl.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hqp.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iqq.yuanzhike.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eah.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yek.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ufs.haohaochexian.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yol.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://ugq.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://ryw.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://oqk.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://gkn.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://ipt.shuidangran.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nxp.cashguo.top

Go:   encoding/gob
来源：http://occ.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://xby.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nec.jinqigfzy.top

================================================================================
来源：http://fgk.tarul.cn

L. 网络请求
来源：http://kkq.yvedp.cn

================================================================================
来源：http://izi.hcnkem.com

[L01] 发送 GET 请求
来源：http://sad.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ggq.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ron.snrcjt.cn

JS:   await fetch(url)
来源：http://jmc.dashuyun.cn

TS:   await fetch(url)
来源：http://lsc.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://umr.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://vgd.nwbrower.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xpp.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wjh.bjfxy.top

[L02] 发送 POST JSON
来源：http://ngw.nanxuanxn.top

Py:   requests.post(url, json={"a": 1})
来源：http://aqr.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ytm.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sem.yangfankeji.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ovk.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uza.yuxming.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nsd.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://phm.vqdsnc.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cpv.zhengqikj.top

[L03] 设置自定义请求头
来源：http://vzz.yueranfly.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://srx.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ias.andypj.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bfn.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ifh.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gln.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vtk.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://law.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wtt.shanyushiyangkeji.top

[L04] 设置超时
来源：http://lnh.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://dqf.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wqr.xuetiantiany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jpe.xuanzx.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fpj.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qnz.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jxr.chenjidiqi.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zyh.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mrs.nwbrower.top

[L05] 上传文件（multipart）
来源：http://uzz.gogol.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tli.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tmq.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rfc.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wss.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yji.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ysd.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gmu.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mhc.havefunace.top

[L06] 解析响应为 JSON
来源：http://ksk.xuanzx.com

Py:   resp.json()
来源：http://dzu.sysykeji.top

PHP:  json_decode($body, true);
来源：http://jbx.yfazqb.com

JS:   await resp.json()
来源：http://qhm.yangfankeji.com

TS:   await resp.json()
来源：http://ezs.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pkd.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://drd.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://ajk.cdnleiting.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xui.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://dcc.yj20258.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dju.xingfuxueyuan.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dor.316326.xyz

JS:   resp.ok;  resp.status
来源：http://xxg.hongshengwenyu.top

TS:   resp.ok;  resp.status
来源：http://jgy.zhoulong.xyz

Java: resp.statusCode()
来源：http://igp.hcnkem.com

Go:   resp.StatusCode
来源：http://xby.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://aso.ybcxt.top

C#:   (int)resp.StatusCode
来源：http://ulh.hywenlv.cn

[L08] 并发请求多个地址
来源：http://chn.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wig.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://hjb.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nti.birdmap.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wir.hnqzz.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sje.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cuj.hnxiangtu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://obu.hnxiangtu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://isc.hysaishi.cn

================================================================================
来源：http://sws.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://mej.xylfe.cn

================================================================================
来源：http://nas.bjfxy.top

[M01] 读取命令行参数
来源：http://qnm.hysaishi.cn

Py:   sys.argv[1:]
来源：http://pko.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://lqw.yueranfly.top

JS:   process.argv.slice(2)
来源：http://cfp.cashguo.top

TS:   process.argv.slice(2)
来源：http://rug.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://ete.chenlongwang.top

Go:   os.Args[1:]
来源：http://kay.yuxming.cn

Ruby: ARGV
来源：http://wwa.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://trc.52xcode.cn

[M02] 读取环境变量
来源：http://qdq.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://qtm.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vkn.gotoacloud.top

JS:   process.env.HOME
来源：http://jar.svipenyu.cn

TS:   process.env.HOME
来源：http://eli.sweek.top

Java: System.getenv("HOME")
来源：http://uwr.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hbh.jianghu66.top

Ruby: ENV["HOME"]
来源：http://ysm.zhixingplan.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hoa.yj20258.top

[M03] 执行外部命令
来源：http://imj.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hai.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yka.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://apr.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mgn.chenlongwang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kin.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yyz.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://mxf.pycfn.com

C#:   Process.Start("ls", "-l");
来源：http://gee.yangfankeji.com

[M04] 获取当前工作目录
来源：http://ipu.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://lua.dianchejie.cn

PHP:  getcwd();
来源：http://qxo.zhijiandao.cn

JS:   process.cwd()
来源：http://zop.sysykeji.top

TS:   process.cwd()
来源：http://imp.aizwys.cn

Java: Path.of("").toAbsolutePath()
来源：http://oee.birdmap.top

Go:   os.Getwd()
来源：http://yec.shanyushiyangkeji.top

Ruby: Dir.pwd
来源：http://sbd.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://igp.meibo888.top

[M05] 设置退出码
来源：http://vsp.ppjwa.cn

Py:   sys.exit(1)
来源：http://upj.nwbrower.top

PHP:  exit(1);
来源：http://ebl.shzxlz.cn

JS:   process.exit(1)
来源：http://kwd.guowangkeji.top

TS:   process.exit(1)
来源：http://deu.jqgfzy.top

Java: System.exit(1)
来源：http://paj.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://pzp.xziqi.cn

Ruby: exit 1
来源：http://xae.zdbjq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kte.gotoacloud.top

[M06] 向标准错误输出
来源：http://isi.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://dts.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fnm.tian-w.cn

JS:   console.error("err")
来源：http://ggh.hfpthk.cn

TS:   console.error("err")
来源：http://jvn.tanke756.top

Java: System.err.println("err")
来源：http://cck.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://avk.uphjek.com

Ruby: warn "err"
来源：http://ttq.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://oeq.daxiang520.top

[M07] 判断是否为主入口
来源：http://mdm.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://sou.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oea.zhijiandao.cn

JS:   require.main === module
来源：http://jnn.jinyuanbaomall.cn

TS:   require.main === module
来源：http://swx.tianlin.xyz

Java: public static void main(String[] args)
来源：http://ksv.snrcjt.cn

Go:   func main()
来源：http://vwu.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jgf.jlsjyb.cn

C#:   static void Main(string[] args)
来源：http://atk.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://afs.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://amm.uphjek.com

PHP:  PHP_OS;  phpversion();
来源：http://fai.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://ghy.tanke756.top

TS:   process.platform;  process.version
来源：http://grb.xylfe.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fkf.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tpc.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ted.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kzy.fengsongda.top

================================================================================
来源：http://rxb.cqqwz.cn

N. 数据结构与算法
来源：http://ozf.zhengqikj.top

================================================================================
来源：http://skj.hammf.cn

[N01] 二分查找（有序数组）
来源：http://tbx.yj20258.top

Py:   bisect.bisect_left(arr, x)
来源：http://eeh.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://och.shzxlz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wlo.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eio.ivvv.top

Java: Arrays.binarySearch(arr, x)
来源：http://upa.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://xpa.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ssi.mhx1999.top

C#:   Array.BinarySearch(arr, x)
来源：http://wlk.daxiang520.top

[N02] 排序（工程实践用内置实现）
来源：http://jfw.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://vei.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hrt.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://iyf.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://foe.uphjek.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kcx.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://gqd.hesvh.cn

Ruby: arr.sort
来源：http://sih.sweek.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dmr.haohaochexian.top

[N03] 快速排序（分治示例）
来源：http://cky.zdbjq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rez.ydzc1.top

PHP:  // 递归实现，或用 usort
来源：http://hid.jianghu66.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://trh.shzxlz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qvj.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://faj.jinyuanbaomall.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xvk.jinqigfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://enh.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://you.xinyue.icu

[N04] 斐波那契数列
来源：http://izc.hysaishi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jze.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xxk.bbcook.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xcr.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://evf.gzhubu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yid.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://whb.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gsj.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://atv.hammf.cn

[N05] 最大公约数
来源：http://ifz.dianchejie.cn

Py:   math.gcd(a, b)
来源：http://ivt.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hpo.dashuyun.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rev.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ysv.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pde.hnqzz.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hmz.birdmap.top

Ruby: a.gcd(b)
来源：http://jdv.wangshuangyany.cn


<!-- 参考信息 -->