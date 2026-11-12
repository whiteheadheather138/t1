代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://dzx.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eyg.316326.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kyd.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jgu.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qgs.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mit.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://svf.vehdjk.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ffk.pycfn.com

================================================================================
来源：http://hhd.jianghu66.top

K. JSON 与序列化
来源：http://ccq.zdqjudy.top

================================================================================
来源：http://gdq.jiagoushi.top

[K01] 对象转 JSON 字符串
来源：http://fqo.yueranfly.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pco.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://flp.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://hqu.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://kwg.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ceg.cucudq.cn

Go:   json.Marshal(obj)
来源：http://gek.cashguo.top

Ruby: obj.to_json                                     // require "json"
来源：http://tns.cdnleiting.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ool.hcnkem.com

[K02] JSON 字符串转对象
来源：http://pzn.feifeiyinyue.top

Py:   json.loads(s)
来源：http://nup.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dyx.haohaochexian.top

JS:   JSON.parse(s)
来源：http://nwn.shuidangran.top

TS:   JSON.parse(s)
来源：http://hnz.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ebv.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://nwl.vqdsnc.cn

Ruby: JSON.parse(s)
来源：http://ehi.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wmn.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://jxo.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vke.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qyq.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gjs.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ygc.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://naz.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dsg.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kjt.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pvu.xuanzx.com

[K04] 读取 JSON 文件
来源：http://dek.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wec.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jvg.wangdashe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uwo.ydzc1.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qzr.quarkkingdee.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rmc.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://opx.ybcxt.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://toq.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://luv.ivvv.top

[K05] 深拷贝对象
来源：http://lic.sxryk.cn

Py:   copy.deepcopy(obj)
来源：http://msf.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://wol.hnqzz.top

JS:   structuredClone(obj)
来源：http://zda.xinyue.icu

TS:   structuredClone(obj)
来源：http://nvc.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xaq.yueranfly.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zmw.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xec.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kqe.shzxlz.cn

[K06] 解析 URL 查询串
来源：http://kef.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ust.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pwq.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qxu.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vho.fehbvm.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uqi.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pah.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nnc.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oop.zhoulong.xyz

[K07] 进制转换
来源：http://itx.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xpw.gogol.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qew.sysykeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zcx.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sxu.fktsv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ooh.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mee.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ism.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vgv.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://tun.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://nrb.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wsr.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://pld.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://udg.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pbq.jinqigfzy.top

Go:   encoding/gob
来源：http://aoi.ydjk.org.cn

Ruby: Marshal.dump(obj)
来源：http://zrq.aibaodan.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dlm.svipenyu.cn

================================================================================
来源：http://gwf.cheryme.top

L. 网络请求
来源：http://aoj.feifeiyinyue.top

================================================================================
来源：http://tbo.yj202588.top

[L01] 发送 GET 请求
来源：http://owd.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vli.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wgd.cheryme.top

JS:   await fetch(url)
来源：http://vnd.zhijiandao.cn

TS:   await fetch(url)
来源：http://hcc.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xqs.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://mxl.shangyingyoupin.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bux.daria6918.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aea.xylfe.cn

[L02] 发送 POST JSON
来源：http://wbz.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://ilx.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qtd.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ogq.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fhz.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://quf.uphjek.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wxf.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://egf.jyoumei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mje.zycfv.cn

[L03] 设置自定义请求头
来源：http://xfo.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dkr.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://otr.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://stg.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lim.ivvv.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qev.yuanzhike.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pzv.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zab.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kig.cdnleiting.top

[L04] 设置超时
来源：http://xvq.tanke756.top

Py:   requests.get(url, timeout=5)
来源：http://esd.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vhk.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zbu.hfpthk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eqs.xuanzx.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ayj.tian-w.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wvc.haohaochexian.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mhj.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cnn.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://otp.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jxa.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xfa.yfazqb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pjj.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://llm.nanxinkj.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cwv.tian-w.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ewj.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dph.tianlin.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yug.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://huo.guowangkeji.top

Py:   resp.json()
来源：http://ann.pycfn.com

PHP:  json_decode($body, true);
来源：http://ize.hfpthk.cn

JS:   await resp.json()
来源：http://hfn.fengsongda.top

TS:   await resp.json()
来源：http://bdy.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ixn.ydjk.org.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rks.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://qof.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ttw.zhongyouzk.top

[L07] 处理 HTTP 状态码
来源：http://vfq.jinghuilouyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tgb.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fhx.birdmap.top

JS:   resp.ok;  resp.status
来源：http://fqi.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://ymg.xinyue.icu

Java: resp.statusCode()
来源：http://scf.vehdjk.com

Go:   resp.StatusCode
来源：http://ddp.gzhubu.top

Ruby: resp.code.to_i
来源：http://oej.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://oyo.jiagoushi.top

[L08] 并发请求多个地址
来源：http://hfc.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tsc.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://nop.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ath.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fiy.chenzaomai.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fjq.9152youxi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bww.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wgw.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yai.yj20258.top

================================================================================
来源：http://mza.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://pkb.pengpengdd.cyou

================================================================================
来源：http://sjj.zdqjudy.top

[M01] 读取命令行参数
来源：http://qap.sweek.top

Py:   sys.argv[1:]
来源：http://dxs.aizwys.cn

PHP:  $argv;  $argc;
来源：http://cpv.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://era.c1oappe.top

TS:   process.argv.slice(2)
来源：http://qnk.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://soj.snrcjt.cn

Go:   os.Args[1:]
来源：http://enk.hesvh.cn

Ruby: ARGV
来源：http://ckp.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://eil.c1oappe.top

[M02] 读取环境变量
来源：http://maa.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://jko.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zfm.nanxinkj.top

JS:   process.env.HOME
来源：http://dii.cheryme.top

TS:   process.env.HOME
来源：http://lrj.xziqi.cn

Java: System.getenv("HOME")
来源：http://fim.hesvh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kji.jiagoushi.top

Ruby: ENV["HOME"]
来源：http://afc.hysaishi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ksz.fehbvm.com

[M03] 执行外部命令
来源：http://lvd.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hbn.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pth.gaohongyu789.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ujs.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ism.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hrh.ydzc1.top

Go:   exec.Command("ls", "-l").Output()
来源：http://eys.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://jdu.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://lpy.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://pbs.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://eqj.vqdsnc.cn

PHP:  getcwd();
来源：http://lts.pycfn.com

JS:   process.cwd()
来源：http://uio.yj20258888.top

TS:   process.cwd()
来源：http://wff.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://dmk.yj20258.top

Go:   os.Getwd()
来源：http://xvt.birdmap.top

Ruby: Dir.pwd
来源：http://mmy.fengsongda.top

C#:   Directory.GetCurrentDirectory()
来源：http://xof.svipenyu.cn

[M05] 设置退出码
来源：http://yxb.shzxlz.cn

Py:   sys.exit(1)
来源：http://ppc.yj202588.top

PHP:  exit(1);
来源：http://jfc.hcnkem.com

JS:   process.exit(1)
来源：http://ygr.yanxiufei.cn

TS:   process.exit(1)
来源：http://xpg.ydzc1.top

Java: System.exit(1)
来源：http://xcs.hammf.cn

Go:   os.Exit(1)
来源：http://wug.smart0.xyz

Ruby: exit 1
来源：http://ngi.cqqwz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://maz.hcnkem.com

[M06] 向标准错误输出
来源：http://kwa.guowangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://vvu.ehwqpu.com

PHP:  fwrite(STDERR, "err\n");
来源：http://qul.hesvh.cn

JS:   console.error("err")
来源：http://dzs.gotoacloud.top

TS:   console.error("err")
来源：http://twg.chenlongwang.top

Java: System.err.println("err")
来源：http://lud.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hsi.daxiang520.top

Ruby: warn "err"
来源：http://lfa.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://cyg.cqqwz.cn

[M07] 判断是否为主入口
来源：http://qru.xziqi.cn

Py:   if __name__ == "__main__":
来源：http://sih.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nfx.meibo888.top

JS:   require.main === module
来源：http://qdf.316326.xyz

TS:   require.main === module
来源：http://agg.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://mkg.xylfe.cn

Go:   func main()
来源：http://nyk.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dke.xuanzx.com

C#:   static void Main(string[] args)
来源：http://zoi.birdmap.top

[M08] 获取系统与运行时信息
来源：http://qmp.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://fjf.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://woq.nwbrower.top

JS:   process.platform;  process.version
来源：http://tqm.shzxlz.cn

TS:   process.platform;  process.version
来源：http://atl.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://evw.shzxlz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pug.ehwqpu.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nni.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ljc.chenjidiqi.icu

================================================================================
来源：http://xtz.ctjpmb.com

N. 数据结构与算法
来源：http://mkw.jinqigufen.top

================================================================================
来源：http://kfl.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://dqx.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hul.cashguo.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://abt.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aat.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vjt.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uhu.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://wrd.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lzg.guowangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://kyn.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://sbo.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://sgg.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sez.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://haa.zhongyouzk.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sze.daria6918.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://box.xingfuxueyuan.xyz

Go:   slices.Sort(arr)
来源：http://ioz.shzxlz.cn

Ruby: arr.sort
来源：http://fmf.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://whj.hywenlv.cn

[N03] 快速排序（分治示例）
来源：http://czb.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nub.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://ukz.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hjd.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kse.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nek.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://amh.jyoumei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tmv.shuidangran.top

C#:   // 手写递归，或 Array.Sort
来源：http://ujb.tarul.cn

[N04] 斐波那契数列
来源：http://smm.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://unb.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://znf.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ckd.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cxx.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bcl.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xtw.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://foy.dashuyun.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tvi.sweek.top

[N05] 最大公约数
来源：http://ycw.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://skl.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ycv.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fsc.pycfn.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tsu.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ohn.nwbrower.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lww.ybcxt.top

Ruby: a.gcd(b)
来源：http://czr.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nom.jlsjyb.cn

[N06] 判断回文字符串
来源：http://dko.svipenyu.cn

Py:   s == s[::-1]
来源：http://cgs.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://cmk.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://fsb.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://czh.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mfl.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://owh.ydjk.org.cn

Ruby: s == s.reverse
来源：http://luu.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yrw.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://hno.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uzf.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tpi.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mkc.zhixingplan.top

TS:   // 手写 Map<string, number>
来源：http://xgv.sjlbkw.cn

Java: // 手写 HashMap
来源：http://odv.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://rzb.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://epc.shanyushiyangtech.top

C#:   // 手写 Dictionary<int, int>
来源：http://toa.hongshengwenyu.top

[N08] 生成全排列
来源：http://rtq.bbcook.cn


<!-- 参考信息 -->