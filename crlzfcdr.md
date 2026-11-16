代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://ilx.xinyue.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zql.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rrd.yj202588.top

Ruby: d1 < d2;  d1 == d2
来源：http://exp.kuanghao11.cn

C#:   d1 < d2;  d1 == d2
来源：http://gcc.vqdsnc.cn

[J08] 提取年月日与星期
来源：http://kht.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pgr.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xlc.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zhg.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hbr.sufxvd.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qxu.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yql.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mma.xingfuxueyuan.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://avw.meibo888.top

[J09] 时区处理
来源：http://omi.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://owl.cucudq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wqw.havefunace.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uhg.shangyingyoupin.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kbd.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lwp.yj20258.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gmu.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vct.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xjx.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://sey.wangdashe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kfb.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ewx.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qsg.xuanzx.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://izi.daria6918.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cqo.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gso.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dol.ydjk.org.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cap.shangyingyoupin.top

================================================================================
来源：http://psx.zhoulong.xyz

K. JSON 与序列化
来源：http://egj.hammf.cn

================================================================================
来源：http://svj.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://qlo.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mmy.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ale.ivvv.top

JS:   JSON.stringify(obj)
来源：http://tjo.jinyuanbaomall.cn

TS:   JSON.stringify(obj)
来源：http://ijs.zhengqikj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qyz.yvedp.cn

Go:   json.Marshal(obj)
来源：http://aba.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zrk.nwbrower.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jvp.xuetiantiany.cn

[K02] JSON 字符串转对象
来源：http://xfr.sjlbkw.cn

Py:   json.loads(s)
来源：http://lye.haohaochexian.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lfc.chenlongwang.top

JS:   JSON.parse(s)
来源：http://fnc.tanke756.top

TS:   JSON.parse(s)
来源：http://ole.hfpthk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://frz.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://cui.ydjk.org.cn

Ruby: JSON.parse(s)
来源：http://emd.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://agy.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://fhz.wangshuangyany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qgs.xuetiantiany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qvm.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://vjs.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://htp.hnqzz.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qki.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gqa.yanxiufei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jqo.9152youxi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ufj.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://krf.iojbl.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uhh.ppjwa.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ate.316326.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mhy.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zwc.pengpengdd.cyou

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qru.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gjs.ybcxt.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://toh.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ikg.cqqwz.cn

[K05] 深拷贝对象
来源：http://rmo.meibo888.top

Py:   copy.deepcopy(obj)
来源：http://bsw.yj20258.top

PHP:  unserialize(serialize($obj));
来源：http://ghg.9152youxi.cn

JS:   structuredClone(obj)
来源：http://ieh.aibaodan.cn

TS:   structuredClone(obj)
来源：http://isw.yueranfly.top

Java: // 手写拷贝构造，或序列化往返
来源：http://toh.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ytn.jqgufenzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gqa.yvedp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bcl.nwbrower.top

[K06] 解析 URL 查询串
来源：http://lea.zdqjudy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vhi.tarul.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://omx.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wkr.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hzn.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ztk.chenlongwang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lcz.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gjg.aizwys.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bfb.yangfankeji.com

[K07] 进制转换
来源：http://biw.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wks.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fbn.jiagoushi.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rjg.daxiang520.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bmt.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jhx.yongpay.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cru.yfazqb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ijp.shangyingyoupin.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lyx.cashguo.top

[K08] 二进制序列化（非 JSON）
来源：http://ksa.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://rdr.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cjt.svipenyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://xkw.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://wsf.ydjk.org.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kpj.ywan-chungtsiang.top

Go:   encoding/gob
来源：http://ddv.hongshengwenyu.top

Ruby: Marshal.dump(obj)
来源：http://bcb.chenjidiqi.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://png.jiagoushi.top

================================================================================
来源：http://uwp.wangshuangyany.cn

L. 网络请求
来源：http://uyh.yangfankeji.com

================================================================================
来源：http://dto.zycfv.cn

[L01] 发送 GET 请求
来源：http://zyw.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://spz.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uaw.smart0.xyz

JS:   await fetch(url)
来源：http://yjs.gogol.net.cn

TS:   await fetch(url)
来源：http://yar.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jsw.meibo888.top

Go:   resp, err := http.Get(url)
来源：http://yxy.bbcook.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ppj.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fsm.ydjk.org.cn

[L02] 发送 POST JSON
来源：http://mxh.smart0.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://wik.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fqn.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tci.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eho.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zad.yangfankeji.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uxc.epnwcf.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uan.chenjidiqi.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jqi.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://gta.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mlk.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ker.yangfankeji.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mlp.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sxk.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bqb.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zun.gzhubu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ioi.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hmv.ydzc1.top

[L04] 设置超时
来源：http://blv.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://gla.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hqt.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rev.yj202588.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://njz.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bsv.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yjo.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kyd.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://byp.hammf.cn

[L05] 上传文件（multipart）
来源：http://qkm.shanyushiyangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sdm.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zdx.bbcook.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ymh.jinyuanbaomall.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tqa.iojbl.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ghy.kuanghao11.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jlf.sysykeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cts.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hso.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://zjw.mhx1999.top

Py:   resp.json()
来源：http://igl.sysykeji.top

PHP:  json_decode($body, true);
来源：http://dkn.wangshuangyany.cn

JS:   await resp.json()
来源：http://ygl.smart0.xyz

TS:   await resp.json()
来源：http://gsr.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ceg.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vwd.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://dog.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://spg.snrcjt.cn

[L07] 处理 HTTP 状态码
来源：http://tnw.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yvg.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gno.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://sti.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://puj.hesvh.cn

Java: resp.statusCode()
来源：http://qzu.fehbvm.com

Go:   resp.StatusCode
来源：http://qdl.dianchejie.cn

Ruby: resp.code.to_i
来源：http://nka.haohaochexian.top

C#:   (int)resp.StatusCode
来源：http://eut.gzhubu.top

[L08] 并发请求多个地址
来源：http://ygy.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://isg.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://ewh.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ayo.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kxo.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wtw.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dyh.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ydc.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://krv.316326.xyz

================================================================================
来源：http://yxr.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://yaq.52xcode.cn

================================================================================
来源：http://wot.xziqi.cn

[M01] 读取命令行参数
来源：http://nxc.chenlongwang.top

Py:   sys.argv[1:]
来源：http://eac.bbcook.cn

PHP:  $argv;  $argc;
来源：http://fqe.jqgfzy.top

JS:   process.argv.slice(2)
来源：http://icr.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://jwq.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://ibc.bbcook.cn

Go:   os.Args[1:]
来源：http://ohp.sufxvd.cn

Ruby: ARGV
来源：http://umx.ydzc1.top

C#:   args 数组（Main 方法参数）
来源：http://oey.dashuyun.cn

[M02] 读取环境变量
来源：http://nwf.chenjidiqi.icu

Py:   os.environ.get("HOME")
来源：http://nvc.zhengqikj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hbq.yj20258888.top

JS:   process.env.HOME
来源：http://teb.cheryme.top

TS:   process.env.HOME
来源：http://aqs.chenzaomai.com

Java: System.getenv("HOME")
来源：http://wtn.yonumen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sem.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://ksd.chenzaomai.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ncd.jinqigfzy.top

[M03] 执行外部命令
来源：http://cgr.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xvo.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fmp.shanyushiyangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rvb.chenjidiqi.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://xql.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uqp.zhiwuduotai.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yst.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://iww.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://cwe.ehwqpu.com

[M04] 获取当前工作目录
来源：http://kui.c1oappe.top

Py:   os.getcwd()
来源：http://thf.sjlbkw.cn

PHP:  getcwd();
来源：http://pbd.quarkkingdee.top

JS:   process.cwd()
来源：http://ito.cdnleiting.top

TS:   process.cwd()
来源：http://zyx.xuetiantiany.cn

Java: Path.of("").toAbsolutePath()
来源：http://clh.wangshuangyany.cn

Go:   os.Getwd()
来源：http://ivj.cheryme.top

Ruby: Dir.pwd
来源：http://ogj.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://cio.hysaishi.cn

[M05] 设置退出码
来源：http://xca.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://cuw.jqgufenzy.top

PHP:  exit(1);
来源：http://hfz.hammf.cn

JS:   process.exit(1)
来源：http://ysx.0kj1m.cn

TS:   process.exit(1)
来源：http://tkm.xylfe.cn

Java: System.exit(1)
来源：http://zlg.tian-w.cn

Go:   os.Exit(1)
来源：http://koi.jianghu66.top

Ruby: exit 1
来源：http://zjm.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cgb.fengsongda.top

[M06] 向标准错误输出
来源：http://php.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://xvw.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rhu.hesvh.cn

JS:   console.error("err")
来源：http://euf.aibaodan.cn

TS:   console.error("err")
来源：http://cay.shzxlz.cn

Java: System.err.println("err")
来源：http://lgx.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bjo.iojbl.cn

Ruby: warn "err"
来源：http://fug.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://yla.cucudq.cn

[M07] 判断是否为主入口
来源：http://vnf.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://psh.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bqr.yj20258888.top

JS:   require.main === module
来源：http://kwc.zhixingplan.top

TS:   require.main === module
来源：http://fyj.yangfankeji.com

Java: public static void main(String[] args)
来源：http://fwf.xylfe.cn

Go:   func main()
来源：http://evl.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tlz.yonumen.top

C#:   static void Main(string[] args)
来源：http://yps.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://pxd.daxiang520.top

Py:   platform.system();  platform.python_version()
来源：http://ybr.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://kkz.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://mrr.fehbvm.com

TS:   process.platform;  process.version
来源：http://pib.iojbl.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bcp.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bzj.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pln.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hkm.gaohongyu789.top

================================================================================
来源：http://dne.hysaishi.cn

N. 数据结构与算法
来源：http://qtl.bjfxy.top

================================================================================
来源：http://ueh.316326.xyz

[N01] 二分查找（有序数组）
来源：http://nxx.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://faq.cucudq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pzv.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vdf.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wiw.ydzc1.top

Java: Arrays.binarySearch(arr, x)
来源：http://qba.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://fcg.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://kfy.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://jqp.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://vtd.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://kpi.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jgd.dashuyun.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xzk.cucudq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rkm.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kpt.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://hey.316326.xyz

Ruby: arr.sort
来源：http://olw.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nle.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://ymc.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qop.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://zes.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qbm.dianchejie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://usw.zdqjudy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ulz.shangyingyoupin.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uzg.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cam.tanke756.top

C#:   // 手写递归，或 Array.Sort
来源：http://lem.dashuyun.cn

[N04] 斐波那契数列
来源：http://thh.ybcxt.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vcq.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yoa.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xai.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dsq.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rdo.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iaq.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://epu.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vwh.hywenlv.cn

[N05] 最大公约数
来源：http://jqt.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://poh.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kwh.guowangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bcx.shanyushiyangkeji.top


<!-- 参考信息 -->