代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://klo.yangfankeji.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gbd.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yes.hfpthk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://isy.wangdashe.top

C#:   d1 < d2;  d1 == d2
来源：http://azt.gogol.net.cn

[J08] 提取年月日与星期
来源：http://jcr.jinghuilouyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ati.daxiang520.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ipf.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gtc.zhaomingkeji.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bmk.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bmp.0kj1m.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ece.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://awg.xuetiantiany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://yhq.ctjpmb.com

[J09] 时区处理
来源：http://cjs.nanxuanxn.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lxc.xziqi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jxf.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vzn.jyoumei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ozr.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sbl.xylfe.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hpn.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yct.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ugr.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://rii.tianlin.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ksw.fehbvm.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bhe.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hdq.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oew.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mev.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hxu.svipenyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tcr.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hzp.chenjidiqi.icu

================================================================================
来源：http://kyq.cheryme.top

K. JSON 与序列化
来源：http://xss.pycfn.com

================================================================================
来源：http://hvk.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://hai.0kj1m.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fhx.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yjg.nwbrower.top

JS:   JSON.stringify(obj)
来源：http://gnd.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://sxi.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mwg.yj202588.top

Go:   json.Marshal(obj)
来源：http://ecf.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://yxh.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cbg.aizwys.cn

[K02] JSON 字符串转对象
来源：http://tpc.dianchejie.cn

Py:   json.loads(s)
来源：http://nds.vqdsnc.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kpr.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://obm.snrcjt.cn

TS:   JSON.parse(s)
来源：http://dui.uphjek.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vhf.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://mhu.hammf.cn

Ruby: JSON.parse(s)
来源：http://vxh.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nwy.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://nps.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zex.hongshengwenyu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ljq.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://iyw.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zyo.feifeiyinyue.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oeq.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://izb.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://dez.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mpl.fktsv.cn

[K04] 读取 JSON 文件
来源：http://ufg.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uqa.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tyt.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uwl.cdnleiting.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qhi.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://arj.bbcook.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://uyf.hongshengwenyu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lcg.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qqz.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://bkz.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://vcn.svipenyu.cn

PHP:  unserialize(serialize($obj));
来源：http://yqh.hysaishi.cn

JS:   structuredClone(obj)
来源：http://vce.jqgfzy.top

TS:   structuredClone(obj)
来源：http://ngx.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nxu.vehdjk.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dze.yueranfly.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ujo.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xhs.shanyushiyangtech.top

[K06] 解析 URL 查询串
来源：http://oru.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iiz.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ukx.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pfw.fzhhl.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pme.yj20258.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pbl.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kmb.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hbi.shzxlz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://slt.hesvh.cn

[K07] 进制转换
来源：http://ymk.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tpe.aizwys.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://opw.yvedp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uyk.guowangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bfw.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ves.zhongyouzk.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ybu.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wmg.xziqi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rjb.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://ocy.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://tln.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ahl.hesvh.cn

JS:   v8.serialize(obj)        // Node
来源：http://ylt.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://mvq.ywan-chungtsiang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nfx.0kj1m.cn

Go:   encoding/gob
来源：http://lgi.andypj.xyz

Ruby: Marshal.dump(obj)
来源：http://kjr.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ser.shangyingyoupin.top

================================================================================
来源：http://aig.chenzaomai.com

L. 网络请求
来源：http://ajb.yueranfly.top

================================================================================
来源：http://mdl.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://gia.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jar.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://csh.zhiwuduotai.top

JS:   await fetch(url)
来源：http://ulm.daria6918.cn

TS:   await fetch(url)
来源：http://bqq.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://efy.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://auf.gzhubu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bmg.yongpay.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gxk.guannengcc.top

[L02] 发送 POST JSON
来源：http://yde.sysykeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://syi.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xkw.hysaishi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eiq.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tub.yonumen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://poi.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://noa.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lnl.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tui.xylfe.cn

[L03] 设置自定义请求头
来源：http://ohq.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mut.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nog.guannengcc.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eku.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qaw.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qri.yanxiufei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dcg.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tqu.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://guj.jlsjyb.cn

[L04] 设置超时
来源：http://ciz.hammf.cn

Py:   requests.get(url, timeout=5)
来源：http://cxe.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://frr.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bxj.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oxh.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hzg.zdbjq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vmd.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uwo.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lsq.cucudq.cn

[L05] 上传文件（multipart）
来源：http://tbb.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hub.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jvc.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ptt.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kiz.birdmap.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pbm.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pha.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lgv.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ksb.jiagoushi.top

[L06] 解析响应为 JSON
来源：http://iuo.kuanghao11.cn

Py:   resp.json()
来源：http://jie.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://mkl.52xcode.cn

JS:   await resp.json()
来源：http://mec.tianlin.xyz

TS:   await resp.json()
来源：http://xwy.tanke756.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dsm.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ohk.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://dst.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dgf.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://bpa.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tdy.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wgw.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://nyb.ivvv.top

TS:   resp.ok;  resp.status
来源：http://vtl.zdbjq.cn

Java: resp.statusCode()
来源：http://qhl.9152youxi.cn

Go:   resp.StatusCode
来源：http://fop.jianghu66.top

Ruby: resp.code.to_i
来源：http://cmp.xuetiantiany.cn

C#:   (int)resp.StatusCode
来源：http://ors.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://ivd.sufxvd.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zzm.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://xws.ydzc1.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mlv.xylfe.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wif.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://txq.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tpl.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://woy.fzhhl.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ypx.guowangkeji.top

================================================================================
来源：http://gqj.quarkkingdee.top

M. 命令行 / 进程 / 环境
来源：http://ajs.quarkkingdee.top

================================================================================
来源：http://myk.chenzaomai.com

[M01] 读取命令行参数
来源：http://giu.iojbl.cn

Py:   sys.argv[1:]
来源：http://mpf.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://jkg.fktsv.cn

JS:   process.argv.slice(2)
来源：http://yzd.jqgufenzy.top

TS:   process.argv.slice(2)
来源：http://ffs.hammf.cn

Java: args 数组（main 方法参数）
来源：http://dfs.vehdjk.com

Go:   os.Args[1:]
来源：http://ptx.birdmap.top

Ruby: ARGV
来源：http://bds.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://hvz.hnxiangtu.top

[M02] 读取环境变量
来源：http://owh.sysykeji.top

Py:   os.environ.get("HOME")
来源：http://ehb.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://asm.tian-w.cn

JS:   process.env.HOME
来源：http://koi.hysaishi.cn

TS:   process.env.HOME
来源：http://kcy.dashuyun.cn

Java: System.getenv("HOME")
来源：http://jcf.yj202588.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mcq.tanke756.top

Ruby: ENV["HOME"]
来源：http://hak.yongpay.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iqt.kuanghao11.cn

[M03] 执行外部命令
来源：http://gmm.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ydy.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mfj.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://oba.ydzc1.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wjp.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sax.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lfu.jinqigfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://cuw.sufxvd.cn

C#:   Process.Start("ls", "-l");
来源：http://dhl.52xcode.cn

[M04] 获取当前工作目录
来源：http://ecx.cucudq.cn

Py:   os.getcwd()
来源：http://mdr.yangfankeji.com

PHP:  getcwd();
来源：http://doo.ivvv.top

JS:   process.cwd()
来源：http://rvi.yfazqb.com

TS:   process.cwd()
来源：http://zpg.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://sjn.smart0.xyz

Go:   os.Getwd()
来源：http://saj.yuxming.cn

Ruby: Dir.pwd
来源：http://koz.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ksh.xinyue.icu

[M05] 设置退出码
来源：http://jck.yanxiufei.cn

Py:   sys.exit(1)
来源：http://vcx.yonumen.top

PHP:  exit(1);
来源：http://sft.zhoulong.xyz

JS:   process.exit(1)
来源：http://zwf.dianchejie.cn

TS:   process.exit(1)
来源：http://htu.xingfuxueyuan.xyz

Java: System.exit(1)
来源：http://kbo.guowangkeji.top

Go:   os.Exit(1)
来源：http://uib.hcnkem.com

Ruby: exit 1
来源：http://hsz.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wfn.zhongyouzk.top

[M06] 向标准错误输出
来源：http://azg.sxryk.cn

Py:   print("err", file=sys.stderr)
来源：http://oht.316326.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ztx.tarul.cn

JS:   console.error("err")
来源：http://miu.uphjek.com

TS:   console.error("err")
来源：http://txz.jinyuanbaomall.cn

Java: System.err.println("err")
来源：http://wja.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mhq.jqgfzy.top

Ruby: warn "err"
来源：http://tfc.nanxuanxn.top

C#:   Console.Error.WriteLine("err")
来源：http://aud.dianchejie.cn

[M07] 判断是否为主入口
来源：http://pcz.havefunace.top

Py:   if __name__ == "__main__":
来源：http://ycp.zhoulong.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wuo.aizwys.cn

JS:   require.main === module
来源：http://btl.316326.xyz

TS:   require.main === module
来源：http://eej.hysaishi.cn

Java: public static void main(String[] args)
来源：http://gbq.nwbrower.top

Go:   func main()
来源：http://ptk.guannengcc.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bhr.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://hfz.bbcook.cn

[M08] 获取系统与运行时信息
来源：http://qhw.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://xcz.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://nmw.yangfankeji.com

JS:   process.platform;  process.version
来源：http://los.sxryk.cn

TS:   process.platform;  process.version
来源：http://bci.0kj1m.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://juc.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hen.fanxiaobao.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wwe.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://qzn.zdqjudy.top

================================================================================
来源：http://nop.zhongyouzk.top

N. 数据结构与算法
来源：http://lxc.cashguo.top

================================================================================
来源：http://msl.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://ixj.gogol.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://prm.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ocu.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nzy.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://otx.vehdjk.com

Java: Arrays.binarySearch(arr, x)
来源：http://aep.havefunace.top

Go:   sort.SearchInts(arr, x)
来源：http://xhb.andypj.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://spe.shzxlz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vbw.guowangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://xas.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://ykk.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ezu.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fmr.hywenlv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bjw.jiagoushi.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zkn.yonumen.top

Go:   slices.Sort(arr)
来源：http://iic.chenzaomai.com

Ruby: arr.sort
来源：http://ixo.aibaodan.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wns.nanxuanxn.top

[N03] 快速排序（分治示例）
来源：http://cwm.tianlin.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fqj.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://all.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sve.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tzm.ehwqpu.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hgi.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cnj.aibaodan.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sst.sweek.top

C#:   // 手写递归，或 Array.Sort
来源：http://ggp.yuanzhike.top

[N04] 斐波那契数列
来源：http://wte.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uwo.tanke756.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ith.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://njm.yj202588.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ago.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bea.vehdjk.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nrf.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zug.zhaomingkeji.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fns.jqgufenzy.top

[N05] 最大公约数
来源：http://cmr.0kj1m.cn

Py:   math.gcd(a, b)
来源：http://giu.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jqx.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hun.kuanghao11.cn


<!-- 参考信息 -->