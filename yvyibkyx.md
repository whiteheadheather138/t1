代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qxi.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nhu.tian-w.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cof.dashuyun.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fky.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wyh.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ovl.tarul.cn

[J09] 时区处理
来源：http://sli.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mby.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sqy.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cdg.fktsv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pyd.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iyd.feifeiyinyue.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://llr.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://wru.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uxc.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://voh.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kxk.epnwcf.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bef.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qmn.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vav.yanxiufei.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://phc.tian-w.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cax.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://obb.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ncz.hammf.cn

================================================================================
来源：http://zyg.guowangkeji.top

K. JSON 与序列化
来源：http://ipk.yangfankeji.com

================================================================================
来源：http://lpc.cqqwz.cn

[K01] 对象转 JSON 字符串
来源：http://ers.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yui.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qjl.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://pqe.yuanzhike.top

TS:   JSON.stringify(obj)
来源：http://mpm.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ndy.zdbjq.cn

Go:   json.Marshal(obj)
来源：http://vim.yonumen.top

Ruby: obj.to_json                                     // require "json"
来源：http://rzz.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zaa.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://itc.epnwcf.com

Py:   json.loads(s)
来源：http://xlw.andypj.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://axp.cheryme.top

JS:   JSON.parse(s)
来源：http://hof.fktsv.cn

TS:   JSON.parse(s)
来源：http://wma.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sdy.zhoulong.xyz

Go:   json.Unmarshal(data, &v)
来源：http://yqv.yvedp.cn

Ruby: JSON.parse(s)
来源：http://gzy.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mni.gaohongyu789.top

[K03] JSON 美化输出（带缩进）
来源：http://uus.gzhubu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bds.zhixingplan.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rlx.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xgl.bjfxy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dww.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yss.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ejt.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://maz.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rqr.yongpay.top

[K04] 读取 JSON 文件
来源：http://pvz.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bhd.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oom.jinqigufen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kfx.bbcook.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pdb.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hom.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://upi.jinqigufen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mji.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cuh.ydjk.org.cn

[K05] 深拷贝对象
来源：http://hhu.jinghuilouyu.cn

Py:   copy.deepcopy(obj)
来源：http://fug.fehbvm.com

PHP:  unserialize(serialize($obj));
来源：http://bui.xziqi.cn

JS:   structuredClone(obj)
来源：http://lbo.aibaodan.cn

TS:   structuredClone(obj)
来源：http://fjx.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://sig.cashguo.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xnk.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mji.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://mtx.cucudq.cn

[K06] 解析 URL 查询串
来源：http://vcl.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eul.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rwi.yonumen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://efl.hammf.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vtg.ctjpmb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hrg.fehbvm.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://ivs.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cxo.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bbc.kuanghao11.cn

[K07] 进制转换
来源：http://ekt.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://okv.zhiwuduotai.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vwy.shuidangran.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ozh.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iyj.jinqigufen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fbm.zhengqikj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gjn.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hzh.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wvn.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://qld.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://pmk.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://oiy.uphjek.com

JS:   v8.serialize(obj)        // Node
来源：http://nmh.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://ujd.yonumen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://czj.yj202588.top

Go:   encoding/gob
来源：http://osu.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://ajq.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rrm.yongpay.top

================================================================================
来源：http://mpu.cucudq.cn

L. 网络请求
来源：http://bki.hongshengwenyu.top

================================================================================
来源：http://yyc.aibaodan.cn

[L01] 发送 GET 请求
来源：http://xmk.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mla.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ykk.pycfn.com

JS:   await fetch(url)
来源：http://bqx.52xcode.cn

TS:   await fetch(url)
来源：http://udl.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://day.sufxvd.cn

Go:   resp, err := http.Get(url)
来源：http://vau.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://uav.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iax.yueranfly.top

[L02] 发送 POST JSON
来源：http://bkc.yongpay.top

Py:   requests.post(url, json={"a": 1})
来源：http://wnr.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hzw.gotoacloud.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fsp.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hqx.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hxw.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qsx.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://acd.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xwv.zhaomingkeji.xyz

[L03] 设置自定义请求头
来源：http://mry.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ich.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wtm.52xcode.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cjn.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://epy.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xpq.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dfq.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fba.gzhubu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hnv.dashuyun.cn

[L04] 设置超时
来源：http://ita.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://yel.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ruy.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://twr.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ixp.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dbd.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fsx.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hkk.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://txr.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://lzo.mhx1999.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qvn.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rge.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://asq.sysykeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://urt.cdnleiting.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://byg.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gdf.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://car.jiagoushi.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pam.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://fzi.jqgfzy.top

Py:   resp.json()
来源：http://yam.daxiang520.top

PHP:  json_decode($body, true);
来源：http://qyz.gotoacloud.top

JS:   await resp.json()
来源：http://ycl.316326.xyz

TS:   await resp.json()
来源：http://rpe.hywenlv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tbz.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://glr.haohaochexian.top

Ruby: JSON.parse(resp.body)
来源：http://wmr.bbcook.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dfx.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://kxh.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dhy.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hdi.xuanzx.com

JS:   resp.ok;  resp.status
来源：http://roh.jinghuilouyu.cn

TS:   resp.ok;  resp.status
来源：http://ttd.yj20258.top

Java: resp.statusCode()
来源：http://wrl.yangfankeji.com

Go:   resp.StatusCode
来源：http://chw.cheryme.top

Ruby: resp.code.to_i
来源：http://xpo.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://rul.yvedp.cn

[L08] 并发请求多个地址
来源：http://vzv.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qwm.zhongyouzk.top

PHP:  curl_multi_init() 系列
来源：http://bua.dianchejie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kos.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yby.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gpc.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vxs.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jjz.quarkkingdee.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zyo.xuetiantiany.cn

================================================================================
来源：http://vyh.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://usi.jqgufenzy.top

================================================================================
来源：http://uur.yj20258.top

[M01] 读取命令行参数
来源：http://hdv.jinqigufen.top

Py:   sys.argv[1:]
来源：http://ong.cheryme.top

PHP:  $argv;  $argc;
来源：http://hpe.epnwcf.com

JS:   process.argv.slice(2)
来源：http://uyt.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://vse.zdbjq.cn

Java: args 数组（main 方法参数）
来源：http://gzs.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://dej.xziqi.cn

Ruby: ARGV
来源：http://hpf.hnqzz.top

C#:   args 数组（Main 方法参数）
来源：http://umg.vqdsnc.cn

[M02] 读取环境变量
来源：http://yov.jinqigfzy.top

Py:   os.environ.get("HOME")
来源：http://tqg.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nfq.52xcode.cn

JS:   process.env.HOME
来源：http://mal.nanxuanxn.top

TS:   process.env.HOME
来源：http://hxn.aibaodan.cn

Java: System.getenv("HOME")
来源：http://mtc.c1oappe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aln.316326.xyz

Ruby: ENV["HOME"]
来源：http://mpw.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uii.zdqjudy.top

[M03] 执行外部命令
来源：http://drd.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qgv.jinqigufen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sgz.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nvw.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cpr.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tdy.hongshengwenyu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://was.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nyq.sysykeji.top

C#:   Process.Start("ls", "-l");
来源：http://qfx.nanxinkj.top

[M04] 获取当前工作目录
来源：http://wna.zhoulong.xyz

Py:   os.getcwd()
来源：http://ygu.ybcxt.top

PHP:  getcwd();
来源：http://ehv.zhijiandao.cn

JS:   process.cwd()
来源：http://svh.haohaochexian.top

TS:   process.cwd()
来源：http://bub.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://ipj.cdnleiting.top

Go:   os.Getwd()
来源：http://dab.yj202588.top

Ruby: Dir.pwd
来源：http://cid.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://vnn.yueranfly.top

[M05] 设置退出码
来源：http://mcd.iojbl.cn

Py:   sys.exit(1)
来源：http://agl.ydzc1.top

PHP:  exit(1);
来源：http://vjf.yj20258888.top

JS:   process.exit(1)
来源：http://kjk.yj20258.top

TS:   process.exit(1)
来源：http://cef.shangyingyoupin.top

Java: System.exit(1)
来源：http://blr.yuanzhike.top

Go:   os.Exit(1)
来源：http://zod.fktsv.cn

Ruby: exit 1
来源：http://uis.zdqjudy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bpl.xingfuxueyuan.xyz

[M06] 向标准错误输出
来源：http://agd.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://uzr.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tcz.cheryme.top

JS:   console.error("err")
来源：http://ucl.shuidangran.top

TS:   console.error("err")
来源：http://cjv.guannengcc.top

Java: System.err.println("err")
来源：http://spt.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ycz.shuidangran.top

Ruby: warn "err"
来源：http://uik.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://sfm.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://qrb.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://ymf.iojbl.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hlc.shanyushiyangkeji.top

JS:   require.main === module
来源：http://znj.fzhhl.top

TS:   require.main === module
来源：http://gzv.yj20258.top

Java: public static void main(String[] args)
来源：http://adj.smart0.xyz

Go:   func main()
来源：http://fcu.hnqzz.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://leq.yvedp.cn

C#:   static void Main(string[] args)
来源：http://per.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://bde.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://tai.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://cek.yongpay.top

JS:   process.platform;  process.version
来源：http://cit.fzhhl.top

TS:   process.platform;  process.version
来源：http://ehz.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dde.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dou.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qvs.yj20258888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cgi.ctjpmb.com

================================================================================
来源：http://wxm.cheryme.top

N. 数据结构与算法
来源：http://sqr.yangfankeji.com

================================================================================
来源：http://nmy.yj202588.top

[N01] 二分查找（有序数组）
来源：http://yle.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://ior.ydjk.org.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zbu.sufxvd.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xzq.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://anj.yj20258.top

Java: Arrays.binarySearch(arr, x)
来源：http://uzh.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://hnh.haohaochexian.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zie.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://crm.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://rlo.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://inz.cheryme.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yub.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hjy.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://che.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hjq.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://acr.zhengqikj.top

Ruby: arr.sort
来源：http://xwf.gzhubu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ibj.yuxming.cn

[N03] 快速排序（分治示例）
来源：http://cph.jinqigufen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lzq.hcnkem.com

PHP:  // 递归实现，或用 usort
来源：http://mdt.uphjek.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://acx.birdmap.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mwx.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ncm.jinqigufen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xke.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bja.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://die.nwbrower.top

[N04] 斐波那契数列
来源：http://kdv.zycfv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oky.redwolf501.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://led.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dgo.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zpu.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tyr.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vig.shangyingyoupin.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ojn.tanke756.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hae.ivvv.top

[N05] 最大公约数
来源：http://pur.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://hri.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kix.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zvj.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uyh.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://szl.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://suu.dianchejie.cn

Ruby: a.gcd(b)
来源：http://ycl.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bte.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://ata.jyoumei.cn

Py:   s == s[::-1]
来源：http://umx.tarul.cn

PHP:  $s === strrev($s);
来源：http://ieh.gogol.net.cn


<!-- 参考信息 -->