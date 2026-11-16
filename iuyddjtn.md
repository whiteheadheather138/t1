代发 wailian999

================================================================================
来源：http://zhh.bjfxy.top

K. JSON 与序列化
来源：http://trk.dashuyun.cn

================================================================================
来源：http://lex.shangyingyoupin.top

[K01] 对象转 JSON 字符串
来源：http://mbk.bjfxy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yyp.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bjx.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://yrk.jqgfzy.top

TS:   JSON.stringify(obj)
来源：http://rwx.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vrs.xuetiantiany.cn

Go:   json.Marshal(obj)
来源：http://tyg.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://ukn.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lki.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://vwr.tanke756.top

Py:   json.loads(s)
来源：http://wyk.nwbrower.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://urg.gzhubu.top

JS:   JSON.parse(s)
来源：http://dbt.ehwqpu.com

TS:   JSON.parse(s)
来源：http://mgf.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fpy.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://lgj.hongshengwenyu.top

Ruby: JSON.parse(s)
来源：http://agj.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wwp.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://khb.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fjn.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lzu.cashguo.top

JS:   JSON.stringify(obj, null, 2)
来源：http://utw.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ikn.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tpd.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mvq.daria6918.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yjm.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jxn.fktsv.cn

[K04] 读取 JSON 文件
来源：http://rln.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tmq.meibo888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wri.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zvo.fanxiaobao.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zim.meibo888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vfh.epnwcf.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hrv.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://dyt.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tzt.guowangkeji.top

[K05] 深拷贝对象
来源：http://vlx.cashguo.top

Py:   copy.deepcopy(obj)
来源：http://tlw.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://atr.hysaishi.cn

JS:   structuredClone(obj)
来源：http://mes.cqqwz.cn

TS:   structuredClone(obj)
来源：http://vyc.jlsjyb.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mrf.ctjpmb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mup.cucudq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nag.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vcf.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://nhe.jyoumei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xcv.tanke756.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mtk.hnqzz.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://noe.yuxming.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cml.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wab.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bev.jyoumei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qtf.tian-w.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ihi.bbcook.cn

[K07] 进制转换
来源：http://hiy.wangdashe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://djx.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jur.kuanghao11.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dwr.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jvp.gzhubu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ggs.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vbf.hysaishi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blj.smart0.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dcc.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://wwm.birdmap.top

Py:   pickle.dumps(obj)
来源：http://vli.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sxx.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://mre.quarkkingdee.top

TS:   v8.serialize(obj)        // Node
来源：http://vhf.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vwk.jianghu66.top

Go:   encoding/gob
来源：http://bza.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://ktr.52xcode.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ywp.yj20258.top

================================================================================
来源：http://uga.hnxiangtu.top

L. 网络请求
来源：http://kwk.sjlbkw.cn

================================================================================
来源：http://uez.dianchejie.cn

[L01] 发送 GET 请求
来源：http://cem.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bix.daria6918.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://psj.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://hcw.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://vuj.hongshengwenyu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tjc.chenzaomai.com

Go:   resp, err := http.Get(url)
来源：http://ntr.bbcook.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://foz.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://igm.aizwys.cn

[L02] 发送 POST JSON
来源：http://cig.birdmap.top

Py:   requests.post(url, json={"a": 1})
来源：http://ksc.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ytp.zdqjudy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aif.dashuyun.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://itf.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bks.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gsr.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mir.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sjd.cucudq.cn

[L03] 设置自定义请求头
来源：http://wdg.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gwy.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kck.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rwk.nwbrower.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ann.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gxx.cqqwz.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pyl.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eyj.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bqr.ehwqpu.com

[L04] 设置超时
来源：http://ijq.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://moe.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hie.epnwcf.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hlq.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bfo.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xke.jlsjyb.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vma.zhiwuduotai.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://syl.pengpengdd.cyou

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iao.hesvh.cn

[L05] 上传文件（multipart）
来源：http://kwu.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ixt.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hmo.yuxming.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ycr.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rsl.gzhubu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tgq.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qdd.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tct.gogol.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jeb.smart0.xyz

[L06] 解析响应为 JSON
来源：http://oul.c1oappe.top

Py:   resp.json()
来源：http://hqh.redwolf501.top

PHP:  json_decode($body, true);
来源：http://stc.nanxinkj.top

JS:   await resp.json()
来源：http://oqw.chenlongwang.top

TS:   await resp.json()
来源：http://eln.smart0.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mlr.cucudq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ivn.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://ejb.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://icw.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://uqo.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://awg.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iys.epnwcf.com

JS:   resp.ok;  resp.status
来源：http://yis.pengpengdd.cyou

TS:   resp.ok;  resp.status
来源：http://fhe.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://nev.zhongyouzk.top

Go:   resp.StatusCode
来源：http://lje.wangshuangyany.cn

Ruby: resp.code.to_i
来源：http://wzd.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://hdd.yuanzhike.top

[L08] 并发请求多个地址
来源：http://qnp.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dhr.ppjwa.cn

PHP:  curl_multi_init() 系列
来源：http://rbj.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bpy.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lzl.andypj.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tny.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sjo.yfazqb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://foo.ehwqpu.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mja.chenlongwang.top

================================================================================
来源：http://zym.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://wrp.epnwcf.com

================================================================================
来源：http://gru.feifeiyinyue.top

[M01] 读取命令行参数
来源：http://gmj.gotoacloud.top

Py:   sys.argv[1:]
来源：http://sec.bjfxy.top

PHP:  $argv;  $argc;
来源：http://lgx.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://ted.52xcode.cn

TS:   process.argv.slice(2)
来源：http://hsb.vqdsnc.cn

Java: args 数组（main 方法参数）
来源：http://eni.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://gao.jyoumei.cn

Ruby: ARGV
来源：http://ofw.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://lrk.shuidangran.top

[M02] 读取环境变量
来源：http://tjt.vqdsnc.cn

Py:   os.environ.get("HOME")
来源：http://inx.zhongyouzk.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xop.birdmap.top

JS:   process.env.HOME
来源：http://kfh.bbcook.cn

TS:   process.env.HOME
来源：http://ckd.xylfe.cn

Java: System.getenv("HOME")
来源：http://jpk.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vev.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://siy.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vuu.hysaishi.cn

[M03] 执行外部命令
来源：http://nud.sjlbkw.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zzv.pycfn.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zdy.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bmm.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://pkj.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ftv.dianchejie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://emc.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://vre.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://nyr.havefunace.top

[M04] 获取当前工作目录
来源：http://gqh.xylfe.cn

Py:   os.getcwd()
来源：http://spk.dianchejie.cn

PHP:  getcwd();
来源：http://ovp.ivvv.top

JS:   process.cwd()
来源：http://fam.smart0.xyz

TS:   process.cwd()
来源：http://wfb.smart0.xyz

Java: Path.of("").toAbsolutePath()
来源：http://xdb.ybcxt.top

Go:   os.Getwd()
来源：http://lvs.daxiang520.top

Ruby: Dir.pwd
来源：http://ujs.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://sic.cqqwz.cn

[M05] 设置退出码
来源：http://ngk.yj20258.top

Py:   sys.exit(1)
来源：http://shr.yj20258888.top

PHP:  exit(1);
来源：http://jwx.shuidangran.top

JS:   process.exit(1)
来源：http://ako.yvedp.cn

TS:   process.exit(1)
来源：http://yeg.aibaodan.cn

Java: System.exit(1)
来源：http://xcf.0kj1m.cn

Go:   os.Exit(1)
来源：http://jio.hysaishi.cn

Ruby: exit 1
来源：http://qhv.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mgc.ivvv.top

[M06] 向标准错误输出
来源：http://lde.yongpay.top

Py:   print("err", file=sys.stderr)
来源：http://lxj.hywenlv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bnl.316326.xyz

JS:   console.error("err")
来源：http://nrz.hysaishi.cn

TS:   console.error("err")
来源：http://amx.0kj1m.cn

Java: System.err.println("err")
来源：http://bea.ppjwa.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bbp.dianchejie.cn

Ruby: warn "err"
来源：http://ixa.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://ltb.havefunace.top

[M07] 判断是否为主入口
来源：http://yeb.yj20258888.top

Py:   if __name__ == "__main__":
来源：http://drk.ctjpmb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rqw.havefunace.top

JS:   require.main === module
来源：http://ots.sxryk.cn

TS:   require.main === module
来源：http://fql.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://gjb.hywenlv.cn

Go:   func main()
来源：http://sef.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ijw.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://sfs.pengpengdd.cyou

[M08] 获取系统与运行时信息
来源：http://uyh.zycfv.cn

Py:   platform.system();  platform.python_version()
来源：http://har.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://vss.hongshengwenyu.top

JS:   process.platform;  process.version
来源：http://hkj.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://pec.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qrn.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xxg.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nta.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://ybs.dianchejie.cn

================================================================================
来源：http://rps.ywan-chungtsiang.top

N. 数据结构与算法
来源：http://zkb.ydzc1.top

================================================================================
来源：http://xoo.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://yiw.cdnleiting.top

Py:   bisect.bisect_left(arr, x)
来源：http://jhy.yuanzhike.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fds.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kfy.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qpx.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://huf.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://wda.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mrx.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://ltr.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://zmb.cashguo.top

Py:   sorted(arr);  arr.sort()
来源：http://vpp.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vty.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gjf.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bzd.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://idx.c1oappe.top

Go:   slices.Sort(arr)
来源：http://noi.smart0.xyz

Ruby: arr.sort
来源：http://myh.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://tsa.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://roc.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hyd.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://enq.cashguo.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xaq.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vvp.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mqj.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://few.daxiang520.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bja.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://pkx.birdmap.top

[N04] 斐波那契数列
来源：http://mua.daxiang520.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mdv.wangdashe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://swp.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hjh.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tkx.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yrz.jiagoushi.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://reo.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xcj.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ebr.ydjk.org.cn

[N05] 最大公约数
来源：http://luq.shanyushiyangtech.top

Py:   math.gcd(a, b)
来源：http://gvi.zhijiandao.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qmi.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rrt.jinghuilouyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qtv.fktsv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dkd.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gmo.9152youxi.cn

Ruby: a.gcd(b)
来源：http://thw.zhoulong.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vmo.pengpengdd.cyou

[N06] 判断回文字符串
来源：http://xbt.zhixingplan.top

Py:   s == s[::-1]
来源：http://pjh.tanke756.top

PHP:  $s === strrev($s);
来源：http://ezb.ybcxt.top

JS:   s === [...s].reverse().join("")
来源：http://btg.jinghuilouyu.cn

TS:   s === [...s].reverse().join("")
来源：http://knx.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xtb.redwolf501.top

Go:   // 双指针从两端比较
来源：http://kkb.yongpay.top

Ruby: s == s.reverse
来源：http://wcp.havefunace.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xid.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://mxx.nwbrower.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zba.hammf.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qia.hywenlv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zvx.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://ngn.316326.xyz

Java: // 手写 HashMap
来源：http://pcy.yj20258888.top

Go:   // 手写 map[int]int
来源：http://fcn.tian-w.cn

Ruby: // 手写 Hash
来源：http://aen.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://rab.tianlin.xyz

[N08] 生成全排列
来源：http://eyd.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://ccy.iojbl.cn

PHP:  // 手写递归交换
来源：http://wth.andypj.xyz

JS:   // 手写回溯递归
来源：http://vwc.tanke756.top

TS:   // 手写回溯递归
来源：http://npr.zhoulong.xyz

Java: // 手写回溯递归
来源：http://ozh.chenlongwang.top

Go:   // 手写回溯递归
来源：http://czt.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://cox.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://lpb.fengsongda.top


<!-- 参考信息 -->