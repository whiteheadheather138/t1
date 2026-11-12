代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zkb.aibaodan.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://iuh.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gad.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://exn.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dlo.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sfb.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hee.316326.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zab.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jte.snrcjt.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wpx.fengsongda.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dxg.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://neh.sweek.top

================================================================================
来源：http://ezm.zhengqikj.top

K. JSON 与序列化
来源：http://rpo.jianghu66.top

================================================================================
来源：http://efs.pycfn.com

[K01] 对象转 JSON 字符串
来源：http://iek.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fsk.fengsongda.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vcr.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://fft.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://stf.fanxiaobao.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dzt.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://cnu.yongpay.top

Ruby: obj.to_json                                     // require "json"
来源：http://vht.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://iod.xylfe.cn

[K02] JSON 字符串转对象
来源：http://zbg.gaohongyu789.top

Py:   json.loads(s)
来源：http://lkm.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://klb.cashguo.top

JS:   JSON.parse(s)
来源：http://jcr.sufxvd.cn

TS:   JSON.parse(s)
来源：http://oka.yj202588.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zqs.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://sdf.ivvv.top

Ruby: JSON.parse(s)
来源：http://avq.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://thp.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://xoi.fengsongda.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ifn.sysykeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://djy.hongshengwenyu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wiq.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kji.shangyingyoupin.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iby.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ldh.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://hcd.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vzq.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://kak.sjlbkw.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ccn.vqdsnc.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kei.guowangkeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ony.nanxuanxn.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rxq.ybcxt.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://msu.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lhb.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://eax.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rdb.hnqzz.top

[K05] 深拷贝对象
来源：http://dgu.sxryk.cn

Py:   copy.deepcopy(obj)
来源：http://ofk.vqdsnc.cn

PHP:  unserialize(serialize($obj));
来源：http://ueb.andypj.xyz

JS:   structuredClone(obj)
来源：http://ffj.nwbrower.top

TS:   structuredClone(obj)
来源：http://pyz.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zfa.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zgw.hnxiangtu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rto.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ify.hongshengwenyu.top

[K06] 解析 URL 查询串
来源：http://zkp.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://etv.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rla.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bnz.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mxx.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dlc.gogol.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rsg.yangfankeji.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hnl.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ftt.bbcook.cn

[K07] 进制转换
来源：http://zvi.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cwx.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gzo.zycfv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wai.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oko.xylfe.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vct.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rzl.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gsd.haohaochexian.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nyx.nwbrower.top

[K08] 二进制序列化（非 JSON）
来源：http://jhw.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://rjn.pycfn.com

PHP:  serialize($obj);  unserialize($s);
来源：http://cvw.nanxinkj.top

JS:   v8.serialize(obj)        // Node
来源：http://eag.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://znw.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gyh.ybcxt.top

Go:   encoding/gob
来源：http://nxl.yfazqb.com

Ruby: Marshal.dump(obj)
来源：http://taj.jinghuilouyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qnj.xuanzx.com

================================================================================
来源：http://zdu.pycfn.com

L. 网络请求
来源：http://ygo.havefunace.top

================================================================================
来源：http://yxn.haohaochexian.top

[L01] 发送 GET 请求
来源：http://hsm.bbcook.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zus.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yhf.sweek.top

JS:   await fetch(url)
来源：http://irl.haohaochexian.top

TS:   await fetch(url)
来源：http://dun.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cds.yuxming.cn

Go:   resp, err := http.Get(url)
来源：http://pqd.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tyr.nanxinkj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ofa.jlsjyb.cn

[L02] 发送 POST JSON
来源：http://vnc.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hvk.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://eje.fktsv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://abo.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pcf.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zed.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yhf.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pau.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://opc.sjlbkw.cn

[L03] 设置自定义请求头
来源：http://yot.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fqu.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bdy.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hos.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iko.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vit.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iwp.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bjh.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://syn.xuetiantiany.cn

[L04] 设置超时
来源：http://foi.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://xin.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://amm.wangshuangyany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://arw.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lcc.jqgufenzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bfi.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eqh.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fhb.vqdsnc.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nxv.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://lwz.zhijiandao.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aiq.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zav.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vmq.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://veq.nanxinkj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pmo.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lgg.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mcb.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yyd.fehbvm.com

[L06] 解析响应为 JSON
来源：http://pcv.havefunace.top

Py:   resp.json()
来源：http://wcw.andypj.xyz

PHP:  json_decode($body, true);
来源：http://nyw.hnqzz.top

JS:   await resp.json()
来源：http://tkb.hcnkem.com

TS:   await resp.json()
来源：http://mue.yvedp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://esg.zycfv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://skb.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://yxu.jinqigufen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gph.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://oyp.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hzk.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wpo.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://euo.pycfn.com

TS:   resp.ok;  resp.status
来源：http://mxu.cheryme.top

Java: resp.statusCode()
来源：http://zux.bjfxy.top

Go:   resp.StatusCode
来源：http://fgb.hywenlv.cn

Ruby: resp.code.to_i
来源：http://cah.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://dhf.feifeiyinyue.top

[L08] 并发请求多个地址
来源：http://wow.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tck.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://kfh.zhiwuduotai.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nfs.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zpz.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ayr.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zmt.zdbjq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://twr.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kbz.svipenyu.cn

================================================================================
来源：http://ghd.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://hya.yvedp.cn

================================================================================
来源：http://sgu.xinyue.icu

[M01] 读取命令行参数
来源：http://cry.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://rae.sjlbkw.cn

PHP:  $argv;  $argc;
来源：http://djo.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://mjp.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://ngm.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://huk.yanxiufei.cn

Go:   os.Args[1:]
来源：http://yxn.jqgfzy.top

Ruby: ARGV
来源：http://opw.52xcode.cn

C#:   args 数组（Main 方法参数）
来源：http://hjz.xuanzx.com

[M02] 读取环境变量
来源：http://hgc.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://yzh.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fvi.chenlongwang.top

JS:   process.env.HOME
来源：http://rgo.svipenyu.cn

TS:   process.env.HOME
来源：http://gfv.svipenyu.cn

Java: System.getenv("HOME")
来源：http://aiy.zhijiandao.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wvm.jlsjyb.cn

Ruby: ENV["HOME"]
来源：http://yom.ehwqpu.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vtw.shuidangran.top

[M03] 执行外部命令
来源：http://gnv.feifeiyinyue.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qpq.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://off.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://naf.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jnn.fktsv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jka.hongshengwenyu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ekj.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://vuf.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://dpn.xingfuxueyuan.xyz

[M04] 获取当前工作目录
来源：http://lbr.birdmap.top

Py:   os.getcwd()
来源：http://ssn.jlsjyb.cn

PHP:  getcwd();
来源：http://eis.redwolf501.top

JS:   process.cwd()
来源：http://hvi.smart0.xyz

TS:   process.cwd()
来源：http://gug.yonumen.top

Java: Path.of("").toAbsolutePath()
来源：http://zdo.zdqjudy.top

Go:   os.Getwd()
来源：http://ect.yfazqb.com

Ruby: Dir.pwd
来源：http://ngr.sufxvd.cn

C#:   Directory.GetCurrentDirectory()
来源：http://obh.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://svb.zhoulong.xyz

Py:   sys.exit(1)
来源：http://nuo.tian-w.cn

PHP:  exit(1);
来源：http://jmi.andypj.xyz

JS:   process.exit(1)
来源：http://ttb.ydjk.org.cn

TS:   process.exit(1)
来源：http://bnn.chenlongwang.top

Java: System.exit(1)
来源：http://jrq.tanke756.top

Go:   os.Exit(1)
来源：http://edk.zdqjudy.top

Ruby: exit 1
来源：http://aoq.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uff.jqgfzy.top

[M06] 向标准错误输出
来源：http://ffu.hnxiangtu.top

Py:   print("err", file=sys.stderr)
来源：http://crx.yj20258888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mmv.smart0.xyz

JS:   console.error("err")
来源：http://lqh.hongshengwenyu.top

TS:   console.error("err")
来源：http://yjy.yongpay.top

Java: System.err.println("err")
来源：http://cwb.ehwqpu.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://luq.zhongyouzk.top

Ruby: warn "err"
来源：http://mnl.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://eal.epnwcf.com

[M07] 判断是否为主入口
来源：http://yuw.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://zwk.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uqh.yonumen.top

JS:   require.main === module
来源：http://wod.guannengcc.top

TS:   require.main === module
来源：http://abx.hfpthk.cn

Java: public static void main(String[] args)
来源：http://jlc.gaohongyu789.top

Go:   func main()
来源：http://eog.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://miv.jianghu66.top

C#:   static void Main(string[] args)
来源：http://wok.meibo888.top

[M08] 获取系统与运行时信息
来源：http://wud.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://lqk.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://msy.zhixingplan.top

JS:   process.platform;  process.version
来源：http://lms.xylfe.cn

TS:   process.platform;  process.version
来源：http://ohe.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tzn.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://pbw.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hse.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kzi.cashguo.top

================================================================================
来源：http://nza.guowangkeji.top

N. 数据结构与算法
来源：http://als.tian-w.cn

================================================================================
来源：http://qxo.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://mcg.xuetiantiany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zdk.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jzi.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xin.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gkx.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://axp.dashuyun.cn

Go:   sort.SearchInts(arr, x)
来源：http://frz.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://sjo.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://mli.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://ngi.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://kuu.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dli.cdnleiting.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://msg.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rfl.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wgy.sjlbkw.cn

Go:   slices.Sort(arr)
来源：http://rif.hnqzz.top

Ruby: arr.sort
来源：http://tvr.tarul.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pew.havefunace.top

[N03] 快速排序（分治示例）
来源：http://oes.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kgc.guowangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://ywv.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://azi.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xda.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wab.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pba.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bbs.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cmo.guowangkeji.top

[N04] 斐波那契数列
来源：http://nar.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rth.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mhs.ydzc1.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tmb.gogol.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uwr.kuanghao11.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qcu.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cqq.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uit.iojbl.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kkv.hesvh.cn

[N05] 最大公约数
来源：http://pul.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://whw.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gev.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ets.ivvv.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://isl.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qbw.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fbk.yangfankeji.com

Ruby: a.gcd(b)
来源：http://kzi.tarul.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pcs.tanke756.top

[N06] 判断回文字符串
来源：http://qvy.zdbjq.cn

Py:   s == s[::-1]
来源：http://zyv.dianchejie.cn

PHP:  $s === strrev($s);
来源：http://nji.ybcxt.top

JS:   s === [...s].reverse().join("")
来源：http://scf.shanyushiyangtech.top

TS:   s === [...s].reverse().join("")
来源：http://oua.yonumen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tzm.xingfuxueyuan.xyz

Go:   // 双指针从两端比较
来源：http://qfq.zhengqikj.top

Ruby: s == s.reverse
来源：http://jas.xylfe.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lft.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://phm.jlsjyb.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dgr.tarul.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nob.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://eln.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://mhx.yongpay.top

Java: // 手写 HashMap
来源：http://ypn.hesvh.cn


<!-- 参考信息 -->