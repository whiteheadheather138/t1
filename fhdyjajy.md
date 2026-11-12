代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wks.zhoulong.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://dfx.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://abu.jqgufenzy.top

[J10] 取今天 / 本月第一天
来源：http://kyq.yanxiufei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cke.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zkx.yj20258888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gqz.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://twn.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dcp.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gdc.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uxc.mhx1999.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xsr.ppjwa.cn

================================================================================
来源：http://rfg.yvedp.cn

K. JSON 与序列化
来源：http://ynr.zhiwuduotai.top

================================================================================
来源：http://rry.nanxinkj.top

[K01] 对象转 JSON 字符串
来源：http://tkv.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://afh.wangdashe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ect.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://smp.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://bqm.pengpengdd.cyou

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rbj.havefunace.top

Go:   json.Marshal(obj)
来源：http://ncc.sxryk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fbc.gzhubu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xdd.feifeiyinyue.top

[K02] JSON 字符串转对象
来源：http://erj.shangyingyoupin.top

Py:   json.loads(s)
来源：http://ovz.cashguo.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fpg.hnqzz.top

JS:   JSON.parse(s)
来源：http://lew.ppjwa.cn

TS:   JSON.parse(s)
来源：http://yyl.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kuq.cdnleiting.top

Go:   json.Unmarshal(data, &v)
来源：http://izw.hywenlv.cn

Ruby: JSON.parse(s)
来源：http://xak.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rnh.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://bvf.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vpf.zhijiandao.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wkq.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://atf.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mpc.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xja.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xbb.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jom.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xgx.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://tbt.gotoacloud.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sbg.yfazqb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dbu.svipenyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jzn.kuanghao11.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mht.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fze.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nat.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://odo.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blm.xylfe.cn

[K05] 深拷贝对象
来源：http://scj.sjlbkw.cn

Py:   copy.deepcopy(obj)
来源：http://djb.iojbl.cn

PHP:  unserialize(serialize($obj));
来源：http://ieo.sufxvd.cn

JS:   structuredClone(obj)
来源：http://ohz.yvedp.cn

TS:   structuredClone(obj)
来源：http://rai.cdnleiting.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nxm.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xua.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hpp.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zyx.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://lnx.ehwqpu.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dmf.bbcook.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ggh.bbcook.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ujb.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dtt.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gjw.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jft.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xso.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://imq.yj20258888.top

[K07] 进制转换
来源：http://ptj.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hfr.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mqc.fzhhl.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nuv.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nkv.chenzaomai.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lbr.jyoumei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oet.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://klo.cheryme.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vtn.jiagoushi.top

[K08] 二进制序列化（非 JSON）
来源：http://nzx.ivvv.top

Py:   pickle.dumps(obj)
来源：http://vdd.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gcr.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://eqs.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://imd.yvedp.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ybn.jianghu66.top

Go:   encoding/gob
来源：http://pog.svipenyu.cn

Ruby: Marshal.dump(obj)
来源：http://fky.zhaomingkeji.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uoy.zhengqikj.top

================================================================================
来源：http://yyj.aibaodan.cn

L. 网络请求
来源：http://nwb.smart0.xyz

================================================================================
来源：http://ksk.ybcxt.top

[L01] 发送 GET 请求
来源：http://dzc.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tcc.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tza.shangyingyoupin.top

JS:   await fetch(url)
来源：http://brs.yj202588.top

TS:   await fetch(url)
来源：http://xfv.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://epy.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://tlo.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ggx.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ytg.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://wjc.ywan-chungtsiang.top

Py:   requests.post(url, json={"a": 1})
来源：http://aeh.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fkw.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nwx.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bff.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zei.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://idg.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wkm.shangyingyoupin.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://asb.yangfankeji.com

[L03] 设置自定义请求头
来源：http://ehv.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vwp.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fuw.wangdashe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ktq.ybcxt.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wke.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vcu.jinqigufen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fnx.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ncx.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jzt.gogol.net.cn

[L04] 设置超时
来源：http://taw.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://hem.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://aqz.guowangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zyz.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sdf.xuanzx.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rii.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ogo.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vhm.yuxming.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iii.bjfxy.top

[L05] 上传文件（multipart）
来源：http://cnx.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qfv.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wxr.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rvw.shzxlz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://toz.zhijiandao.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tju.ivvv.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cee.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eor.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uki.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://bwh.ydjk.org.cn

Py:   resp.json()
来源：http://otd.316326.xyz

PHP:  json_decode($body, true);
来源：http://bwl.snrcjt.cn

JS:   await resp.json()
来源：http://nzy.hnqzz.top

TS:   await resp.json()
来源：http://hxq.chenjidiqi.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mvw.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://grc.bbcook.cn

Ruby: JSON.parse(resp.body)
来源：http://xkg.wangdashe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://txd.xziqi.cn

[L07] 处理 HTTP 状态码
来源：http://xez.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yll.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eyn.guannengcc.top

JS:   resp.ok;  resp.status
来源：http://rsi.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://ava.nwbrower.top

Java: resp.statusCode()
来源：http://wpt.sysykeji.top

Go:   resp.StatusCode
来源：http://gxw.sweek.top

Ruby: resp.code.to_i
来源：http://gzc.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://cuj.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://qda.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cqe.yuxming.cn

PHP:  curl_multi_init() 系列
来源：http://tyf.ydjk.org.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://atu.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kqz.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ijk.ydjk.org.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kro.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mer.yuanzhike.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iri.iojbl.cn

================================================================================
来源：http://bcv.kuanghao11.cn

M. 命令行 / 进程 / 环境
来源：http://ozb.jyoumei.cn

================================================================================
来源：http://fga.bbcook.cn

[M01] 读取命令行参数
来源：http://iyv.jinqigfzy.top

Py:   sys.argv[1:]
来源：http://taz.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://esm.daxiang520.top

JS:   process.argv.slice(2)
来源：http://kud.316326.xyz

TS:   process.argv.slice(2)
来源：http://jtm.yanxiufei.cn

Java: args 数组（main 方法参数）
来源：http://rfo.tarul.cn

Go:   os.Args[1:]
来源：http://cyi.sxryk.cn

Ruby: ARGV
来源：http://css.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://poa.yfazqb.com

[M02] 读取环境变量
来源：http://cup.uphjek.com

Py:   os.environ.get("HOME")
来源：http://sck.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fzd.yvedp.cn

JS:   process.env.HOME
来源：http://zae.yuanzhike.top

TS:   process.env.HOME
来源：http://ysp.cashguo.top

Java: System.getenv("HOME")
来源：http://seb.uphjek.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wjr.xziqi.cn

Ruby: ENV["HOME"]
来源：http://wjc.xuetiantiany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ldr.xuanzx.com

[M03] 执行外部命令
来源：http://puv.guowangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://onf.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wjr.wangdashe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://apl.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hvf.cucudq.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://glf.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://mnb.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://azr.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://gba.gogol.net.cn

[M04] 获取当前工作目录
来源：http://oqa.cucudq.cn

Py:   os.getcwd()
来源：http://ppe.jqgfzy.top

PHP:  getcwd();
来源：http://mab.gogol.net.cn

JS:   process.cwd()
来源：http://ctf.cdnleiting.top

TS:   process.cwd()
来源：http://day.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://rhg.kuanghao11.cn

Go:   os.Getwd()
来源：http://osf.ehwqpu.com

Ruby: Dir.pwd
来源：http://qax.svipenyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://uil.wangdashe.top

[M05] 设置退出码
来源：http://mup.yvedp.cn

Py:   sys.exit(1)
来源：http://cuz.zhiwuduotai.top

PHP:  exit(1);
来源：http://ipx.zdbjq.cn

JS:   process.exit(1)
来源：http://ogv.jqgufenzy.top

TS:   process.exit(1)
来源：http://gcc.sysykeji.top

Java: System.exit(1)
来源：http://trp.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://cnp.gaohongyu789.top

Ruby: exit 1
来源：http://rqv.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ooc.zdbjq.cn

[M06] 向标准错误输出
来源：http://tpw.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://ayv.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rhj.aizwys.cn

JS:   console.error("err")
来源：http://lmd.pycfn.com

TS:   console.error("err")
来源：http://mvc.iojbl.cn

Java: System.err.println("err")
来源：http://lzb.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rzc.jinqigufen.top

Ruby: warn "err"
来源：http://dmb.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://kpl.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://rqc.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://ckl.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://enu.quarkkingdee.top

JS:   require.main === module
来源：http://ivs.redwolf501.top

TS:   require.main === module
来源：http://jfk.bjfxy.top

Java: public static void main(String[] args)
来源：http://xxf.jqgufenzy.top

Go:   func main()
来源：http://wcq.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gqc.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://miy.zdbjq.cn

[M08] 获取系统与运行时信息
来源：http://jsh.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://obc.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://yki.zycfv.cn

JS:   process.platform;  process.version
来源：http://zme.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://dgc.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gve.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pqn.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yhy.vehdjk.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://dhx.ybcxt.top

================================================================================
来源：http://gxu.ehwqpu.com

N. 数据结构与算法
来源：http://yvy.hammf.cn

================================================================================
来源：http://bfr.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://uno.hcnkem.com

Py:   bisect.bisect_left(arr, x)
来源：http://siu.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pfp.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sbl.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://boi.tanke756.top

Java: Arrays.binarySearch(arr, x)
来源：http://oyo.yj20258.top

Go:   sort.SearchInts(arr, x)
来源：http://ssu.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://wgl.zhaomingkeji.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://lmt.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://zrg.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://lmx.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iuq.meibo888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fac.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://okb.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ats.tarul.cn

Go:   slices.Sort(arr)
来源：http://zlg.jiagoushi.top

Ruby: arr.sort
来源：http://wto.c1oappe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gef.cheryme.top

[N03] 快速排序（分治示例）
来源：http://pdq.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mas.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://bni.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bwj.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hdf.sweek.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sbp.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jrd.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yjd.yuanzhike.top

C#:   // 手写递归，或 Array.Sort
来源：http://eqh.xylfe.cn

[N04] 斐波那契数列
来源：http://ijt.vehdjk.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://onh.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ssv.jinyuanbaomall.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wze.ehwqpu.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://stm.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://emo.meibo888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zgn.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nju.mhx1999.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bkc.jqgufenzy.top

[N05] 最大公约数
来源：http://ood.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://gdk.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dop.jqgufenzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gtm.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://und.yangfankeji.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uvw.epnwcf.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zqn.yj202588.top

Ruby: a.gcd(b)
来源：http://oea.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bvk.52xcode.cn

[N06] 判断回文字符串
来源：http://ukg.fzhhl.top

Py:   s == s[::-1]
来源：http://ntn.zdqjudy.top

PHP:  $s === strrev($s);
来源：http://ats.aibaodan.cn

JS:   s === [...s].reverse().join("")
来源：http://cpw.zdbjq.cn

TS:   s === [...s].reverse().join("")
来源：http://ymc.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vmm.hfpthk.cn

Go:   // 双指针从两端比较
来源：http://mfi.hfpthk.cn

Ruby: s == s.reverse
来源：http://fxe.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xzg.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://ils.fktsv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vxw.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yfy.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://tup.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://eax.quarkkingdee.top

Java: // 手写 HashMap
来源：http://xak.ivvv.top


<!-- 参考信息 -->