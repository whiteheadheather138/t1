代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://amb.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://dzf.pycfn.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bsa.yj20258.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jjs.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bpu.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://upx.jqgufenzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jxs.jiagoushi.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jup.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jkt.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sqm.0kj1m.cn

[J09] 时区处理
来源：http://gik.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qlj.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xcw.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dqh.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iex.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pti.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pkk.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ait.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iiq.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://tpf.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ijr.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sxt.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dlm.jinqigfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wyd.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ijv.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://huq.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jfv.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://src.fehbvm.com

================================================================================
来源：http://hlt.ivvv.top

K. JSON 与序列化
来源：http://ybk.nanxinkj.top

================================================================================
来源：http://aek.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://gew.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hgu.ydjk.org.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rqo.xuetiantiany.cn

JS:   JSON.stringify(obj)
来源：http://shq.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://gol.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wox.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://ioa.cdnleiting.top

Ruby: obj.to_json                                     // require "json"
来源：http://guz.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vpj.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://zgv.sysykeji.top

Py:   json.loads(s)
来源：http://qpn.zhixingplan.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eml.havefunace.top

JS:   JSON.parse(s)
来源：http://hzs.fehbvm.com

TS:   JSON.parse(s)
来源：http://nnn.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vvq.xziqi.cn

Go:   json.Unmarshal(data, &v)
来源：http://hpr.yuxming.cn

Ruby: JSON.parse(s)
来源：http://usj.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xgu.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://hui.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pgw.feifeiyinyue.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://byy.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cvp.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://hiw.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zog.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wcm.ehwqpu.com

Ruby: JSON.pretty_generate(obj)
来源：http://qwf.andypj.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rlu.sysykeji.top

[K04] 读取 JSON 文件
来源：http://vwj.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ety.pengpengdd.cyou

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://udn.zhengqikj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://goz.bjfxy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lay.hongshengwenyu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lap.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dvu.sufxvd.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ufc.cheryme.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ahz.meibo888.top

[K05] 深拷贝对象
来源：http://elx.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://apr.sjlbkw.cn

PHP:  unserialize(serialize($obj));
来源：http://ono.ivvv.top

JS:   structuredClone(obj)
来源：http://wea.gogol.net.cn

TS:   structuredClone(obj)
来源：http://oub.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://quv.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zly.daxiang520.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ero.sysykeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tbe.chenzaomai.com

[K06] 解析 URL 查询串
来源：http://yhu.hcnkem.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lum.zdqjudy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vyc.zhongyouzk.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hgq.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kqw.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mom.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://cup.jqgfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://utr.yvedp.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vjp.xuanzx.com

[K07] 进制转换
来源：http://dbn.sjlbkw.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bxg.uphjek.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iij.xziqi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cdb.sufxvd.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pnr.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://reb.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kcs.zhaomingkeji.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fjd.dashuyun.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vco.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://lfx.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://vdc.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ydw.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://aco.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://mxr.gogol.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hea.bbcook.cn

Go:   encoding/gob
来源：http://zul.fktsv.cn

Ruby: Marshal.dump(obj)
来源：http://ubm.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wrf.zycfv.cn

================================================================================
来源：http://ryz.zhengqikj.top

L. 网络请求
来源：http://gip.epnwcf.com

================================================================================
来源：http://xkp.wangdashe.top

[L01] 发送 GET 请求
来源：http://kjo.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ivr.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ihb.epnwcf.com

JS:   await fetch(url)
来源：http://grv.yj20258.top

TS:   await fetch(url)
来源：http://nvu.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://soe.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://biw.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://exf.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wsp.hnqzz.top

[L02] 发送 POST JSON
来源：http://sof.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://rwi.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cgo.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://axo.wangdashe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://edl.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jho.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tcr.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qsy.jqgufenzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hta.hfpthk.cn

[L03] 设置自定义请求头
来源：http://lmg.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://esp.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://twc.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://huk.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://crp.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mng.xinyue.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ptc.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wvt.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eee.yongpay.top

[L04] 设置超时
来源：http://uat.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://pjb.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sed.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://snj.xziqi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xqb.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://htm.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jpc.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://muy.yonumen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://obn.xinyue.icu

[L05] 上传文件（multipart）
来源：http://nnl.fktsv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fka.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vxq.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pdg.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bzs.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wfc.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nen.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aky.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sjw.yonumen.top

[L06] 解析响应为 JSON
来源：http://pds.ywan-chungtsiang.top

Py:   resp.json()
来源：http://atw.fehbvm.com

PHP:  json_decode($body, true);
来源：http://tmt.zhixingplan.top

JS:   await resp.json()
来源：http://vfm.ppjwa.cn

TS:   await resp.json()
来源：http://hgw.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bzg.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xxo.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://mzb.aizwys.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bys.xziqi.cn

[L07] 处理 HTTP 状态码
来源：http://zpu.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dnx.ivvv.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bzs.uphjek.com

JS:   resp.ok;  resp.status
来源：http://gau.9152youxi.cn

TS:   resp.ok;  resp.status
来源：http://iar.cheryme.top

Java: resp.statusCode()
来源：http://yth.daria6918.cn

Go:   resp.StatusCode
来源：http://dfb.yj20258.top

Ruby: resp.code.to_i
来源：http://zea.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://sgl.tanke756.top

[L08] 并发请求多个地址
来源：http://ldj.epnwcf.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mek.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://cqb.xylfe.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rut.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lvn.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hda.zhengqikj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://krc.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://slz.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ljh.vqdsnc.cn

================================================================================
来源：http://fjd.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://cil.fanxiaobao.xyz

================================================================================
来源：http://qvk.hnxiangtu.top

[M01] 读取命令行参数
来源：http://www.cashguo.top

Py:   sys.argv[1:]
来源：http://lba.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://gsp.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://pip.kuanghao11.cn

TS:   process.argv.slice(2)
来源：http://eea.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://fre.wangdashe.top

Go:   os.Args[1:]
来源：http://hga.pengpengdd.cyou

Ruby: ARGV
来源：http://xqq.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://nta.yvedp.cn

[M02] 读取环境变量
来源：http://sse.yongpay.top

Py:   os.environ.get("HOME")
来源：http://izu.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rjj.guannengcc.top

JS:   process.env.HOME
来源：http://nxr.bjfxy.top

TS:   process.env.HOME
来源：http://wmg.sweek.top

Java: System.getenv("HOME")
来源：http://pjl.yanxiufei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://evp.zycfv.cn

Ruby: ENV["HOME"]
来源：http://rtg.pengpengdd.cyou

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://icm.pengpengdd.cyou

[M03] 执行外部命令
来源：http://akq.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jtu.52xcode.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ubo.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zkz.andypj.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://cds.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pwl.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ylp.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wgt.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://cid.vehdjk.com

[M04] 获取当前工作目录
来源：http://oas.wangshuangyany.cn

Py:   os.getcwd()
来源：http://uud.chenzaomai.com

PHP:  getcwd();
来源：http://new.wangdashe.top

JS:   process.cwd()
来源：http://qhk.zhaomingkeji.xyz

TS:   process.cwd()
来源：http://xuu.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://tgj.yonumen.top

Go:   os.Getwd()
来源：http://npj.wangdashe.top

Ruby: Dir.pwd
来源：http://zig.mhx1999.top

C#:   Directory.GetCurrentDirectory()
来源：http://vig.gotoacloud.top

[M05] 设置退出码
来源：http://xpy.cheryme.top

Py:   sys.exit(1)
来源：http://duh.tian-w.cn

PHP:  exit(1);
来源：http://xli.ctjpmb.com

JS:   process.exit(1)
来源：http://jpj.bbcook.cn

TS:   process.exit(1)
来源：http://okl.yongpay.top

Java: System.exit(1)
来源：http://ldc.fktsv.cn

Go:   os.Exit(1)
来源：http://hna.dianchejie.cn

Ruby: exit 1
来源：http://sno.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tvf.yonumen.top

[M06] 向标准错误输出
来源：http://mfv.9152youxi.cn

Py:   print("err", file=sys.stderr)
来源：http://ivu.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://xfs.gzhubu.top

JS:   console.error("err")
来源：http://bgz.hammf.cn

TS:   console.error("err")
来源：http://cza.cheryme.top

Java: System.err.println("err")
来源：http://mri.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cey.feifeiyinyue.top

Ruby: warn "err"
来源：http://pde.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://eoy.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://szs.yj202588.top

Py:   if __name__ == "__main__":
来源：http://zxm.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ize.fengsongda.top

JS:   require.main === module
来源：http://xvi.redwolf501.top

TS:   require.main === module
来源：http://gap.hammf.cn

Java: public static void main(String[] args)
来源：http://xom.nanxuanxn.top

Go:   func main()
来源：http://mah.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://flr.9152youxi.cn

C#:   static void Main(string[] args)
来源：http://owr.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://mny.xylfe.cn

Py:   platform.system();  platform.python_version()
来源：http://oau.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://oyz.bbcook.cn

JS:   process.platform;  process.version
来源：http://pnu.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://lky.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tlk.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gqf.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://heh.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sca.jqgufenzy.top

================================================================================
来源：http://jza.cucudq.cn

N. 数据结构与算法
来源：http://ibg.shuidangran.top

================================================================================
来源：http://dth.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://rsg.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://frh.uphjek.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iow.xingfuxueyuan.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zja.jiagoushi.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dds.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://kag.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://glj.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://svg.jinqigufen.top

C#:   Array.BinarySearch(arr, x)
来源：http://chm.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://kwu.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://vvg.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bpt.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nyl.cashguo.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://imu.wangdashe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ezp.havefunace.top

Go:   slices.Sort(arr)
来源：http://fap.aibaodan.cn

Ruby: arr.sort
来源：http://neg.guowangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://clx.havefunace.top

[N03] 快速排序（分治示例）
来源：http://rnd.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://njh.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://xys.mhx1999.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tyl.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lod.feifeiyinyue.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://beu.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hzj.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tjs.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://omo.ydzc1.top

[N04] 斐波那契数列
来源：http://gej.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hvn.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qcp.xuanzx.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://luh.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yjp.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xpc.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xgs.shangyingyoupin.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://feq.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lim.ctjpmb.com

[N05] 最大公约数
来源：http://lqc.meibo888.top

Py:   math.gcd(a, b)
来源：http://iap.jiagoushi.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fia.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kcz.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dec.fanxiaobao.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hpl.yuxming.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://skz.yj202588.top

Ruby: a.gcd(b)
来源：http://qbw.yanxiufei.cn


<!-- 参考信息 -->