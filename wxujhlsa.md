代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ote.tianlin.xyz

Go:   json.Marshal(obj)
来源：http://upe.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://crb.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bwa.pycfn.com

[K02] JSON 字符串转对象
来源：http://pnl.aibaodan.cn

Py:   json.loads(s)
来源：http://sjo.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ijc.fanxiaobao.xyz

JS:   JSON.parse(s)
来源：http://tlg.tanke756.top

TS:   JSON.parse(s)
来源：http://scv.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dbu.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://mtf.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://fhr.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fne.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://knz.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kjb.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://brp.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://eeh.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wyi.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cew.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sez.sweek.top

Ruby: JSON.pretty_generate(obj)
来源：http://the.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wgv.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://bdn.xingfuxueyuan.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sze.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sit.yongpay.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pmb.zhengqikj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ujw.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qlm.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://woi.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://xqj.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ioh.ppjwa.cn

[K05] 深拷贝对象
来源：http://tvh.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://gtw.fktsv.cn

PHP:  unserialize(serialize($obj));
来源：http://wqh.gaohongyu789.top

JS:   structuredClone(obj)
来源：http://qzb.jinyuanbaomall.cn

TS:   structuredClone(obj)
来源：http://hww.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ovi.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tfw.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iic.chenzaomai.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ygn.hammf.cn

[K06] 解析 URL 查询串
来源：http://gab.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qmk.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yvr.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aav.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uvm.uphjek.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://loz.yuxming.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vll.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nqa.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ydw.hcnkem.com

[K07] 进制转换
来源：http://rtx.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dkq.fktsv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cnz.fanxiaobao.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yat.nwbrower.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ogg.zhijiandao.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rxq.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ici.hammf.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ilv.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pqy.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://flm.shanyushiyangkeji.top

Py:   pickle.dumps(obj)
来源：http://fxg.xinyue.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://pcf.ydzc1.top

JS:   v8.serialize(obj)        // Node
来源：http://bhi.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://lld.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tyl.0kj1m.cn

Go:   encoding/gob
来源：http://jry.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://hhv.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wtz.yuanzhike.top

================================================================================
来源：http://wup.havefunace.top

L. 网络请求
来源：http://dvy.feifeiyinyue.top

================================================================================
来源：http://xvi.jqgfzy.top

[L01] 发送 GET 请求
来源：http://sqo.smart0.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gpd.hcnkem.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://viz.yj202588.top

JS:   await fetch(url)
来源：http://gul.yvedp.cn

TS:   await fetch(url)
来源：http://ewc.ybcxt.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://juj.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://crm.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dts.dianchejie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dqi.gogol.net.cn

[L02] 发送 POST JSON
来源：http://dtc.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://zhs.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xur.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dme.nanxuanxn.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eyp.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tib.jinqigfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yjo.svipenyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://guu.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xmv.shuidangran.top

[L03] 设置自定义请求头
来源：http://lfn.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ivo.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eaq.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zmq.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nfk.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qtb.hcnkem.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fal.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ivt.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pxn.zhoulong.xyz

[L04] 设置超时
来源：http://pjg.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://xyc.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oxa.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jvu.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fzt.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://huk.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tkc.zdqjudy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yqw.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ftm.sysykeji.top

[L05] 上传文件（multipart）
来源：http://fiq.pycfn.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://spo.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://oxn.sjlbkw.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vmx.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pss.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wsw.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tcn.tian-w.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lxa.ywan-chungtsiang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xcv.shuidangran.top

[L06] 解析响应为 JSON
来源：http://xul.chenlongwang.top

Py:   resp.json()
来源：http://rms.havefunace.top

PHP:  json_decode($body, true);
来源：http://zbu.hywenlv.cn

JS:   await resp.json()
来源：http://yfd.jinqigfzy.top

TS:   await resp.json()
来源：http://wmn.yj202588.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gxp.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ykv.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://qys.shangyingyoupin.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vxi.yonumen.top

[L07] 处理 HTTP 状态码
来源：http://sex.hywenlv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wca.jlsjyb.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qkl.chenjidiqi.icu

JS:   resp.ok;  resp.status
来源：http://mzq.xziqi.cn

TS:   resp.ok;  resp.status
来源：http://shx.yanxiufei.cn

Java: resp.statusCode()
来源：http://xak.jlsjyb.cn

Go:   resp.StatusCode
来源：http://rsx.sufxvd.cn

Ruby: resp.code.to_i
来源：http://omo.pengpengdd.cyou

C#:   (int)resp.StatusCode
来源：http://qpf.yonumen.top

[L08] 并发请求多个地址
来源：http://zhq.yj202588.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blp.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://gxa.cqqwz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cba.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pjj.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://amy.pengpengdd.cyou

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vtg.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pcd.zdqjudy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qyg.sweek.top

================================================================================
来源：http://rtu.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://qiq.aizwys.cn

================================================================================
来源：http://kbk.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://gxq.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://fuo.fzhhl.top

PHP:  $argv;  $argc;
来源：http://bfk.tarul.cn

JS:   process.argv.slice(2)
来源：http://fmv.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://nhq.sysykeji.top

Java: args 数组（main 方法参数）
来源：http://vme.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://xiq.xuetiantiany.cn

Ruby: ARGV
来源：http://rly.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://pfd.birdmap.top

[M02] 读取环境变量
来源：http://scl.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://fws.ydjk.org.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lzl.jianghu66.top

JS:   process.env.HOME
来源：http://jnp.andypj.xyz

TS:   process.env.HOME
来源：http://hwf.yj20258.top

Java: System.getenv("HOME")
来源：http://nbn.wangdashe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ofa.quarkkingdee.top

Ruby: ENV["HOME"]
来源：http://utc.chenzaomai.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://egg.dashuyun.cn

[M03] 执行外部命令
来源：http://hao.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ldl.wangshuangyany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zxs.zhengqikj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hzt.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://ijm.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hhu.sxryk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://edr.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://xlk.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://iwx.ppjwa.cn

[M04] 获取当前工作目录
来源：http://lpw.uphjek.com

Py:   os.getcwd()
来源：http://bro.cdnleiting.top

PHP:  getcwd();
来源：http://atn.hysaishi.cn

JS:   process.cwd()
来源：http://ult.daria6918.cn

TS:   process.cwd()
来源：http://ohy.fehbvm.com

Java: Path.of("").toAbsolutePath()
来源：http://pde.52xcode.cn

Go:   os.Getwd()
来源：http://erk.zhengqikj.top

Ruby: Dir.pwd
来源：http://ris.jinqigufen.top

C#:   Directory.GetCurrentDirectory()
来源：http://brj.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://vtd.jinqigufen.top

Py:   sys.exit(1)
来源：http://dbd.ehwqpu.com

PHP:  exit(1);
来源：http://xsy.hongshengwenyu.top

JS:   process.exit(1)
来源：http://gov.hcnkem.com

TS:   process.exit(1)
来源：http://fhl.sjlbkw.cn

Java: System.exit(1)
来源：http://gge.chenzaomai.com

Go:   os.Exit(1)
来源：http://qau.sysykeji.top

Ruby: exit 1
来源：http://mfp.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://alm.jqgfzy.top

[M06] 向标准错误输出
来源：http://mbx.xinyue.icu

Py:   print("err", file=sys.stderr)
来源：http://zxi.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dwk.vqdsnc.cn

JS:   console.error("err")
来源：http://mbv.ydzc1.top

TS:   console.error("err")
来源：http://xrm.hfpthk.cn

Java: System.err.println("err")
来源：http://qfl.xuetiantiany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ieh.zhijiandao.cn

Ruby: warn "err"
来源：http://qpw.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://qna.yongpay.top

[M07] 判断是否为主入口
来源：http://uqd.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://qgg.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oti.ydjk.org.cn

JS:   require.main === module
来源：http://ddw.jlsjyb.cn

TS:   require.main === module
来源：http://gmq.yuanzhike.top

Java: public static void main(String[] args)
来源：http://zlj.gzhubu.top

Go:   func main()
来源：http://lba.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jmz.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://hgf.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://aoj.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://oha.cqqwz.cn

PHP:  PHP_OS;  phpversion();
来源：http://uql.yj202588.top

JS:   process.platform;  process.version
来源：http://apk.aizwys.cn

TS:   process.platform;  process.version
来源：http://nen.zhixingplan.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kyw.52xcode.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://crs.ctjpmb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zex.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kzf.gzhubu.top

================================================================================
来源：http://efc.9152youxi.cn

N. 数据结构与算法
来源：http://ycr.ybcxt.top

================================================================================
来源：http://vqb.zdbjq.cn

[N01] 二分查找（有序数组）
来源：http://vgh.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://ffe.zhixingplan.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ttu.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ybi.wangshuangyany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xgg.sweek.top

Java: Arrays.binarySearch(arr, x)
来源：http://wbb.zdqjudy.top

Go:   sort.SearchInts(arr, x)
来源：http://eop.gaohongyu789.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hyw.zhongyouzk.top

C#:   Array.BinarySearch(arr, x)
来源：http://lgi.quarkkingdee.top

[N02] 排序（工程实践用内置实现）
来源：http://nfn.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://bnu.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jac.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://smh.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://iar.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kva.guannengcc.top

Go:   slices.Sort(arr)
来源：http://ecw.yonumen.top

Ruby: arr.sort
来源：http://vrj.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ifb.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://rnh.ybcxt.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vyd.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://puu.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ckt.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://are.pengpengdd.cyou

Java: // 手写递归，或直接用 Arrays.sort
来源：http://spe.ppjwa.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mkm.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vxh.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://ftt.tanke756.top

[N04] 斐波那契数列
来源：http://znl.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nsg.dianchejie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ggo.shuidangran.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yko.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://urb.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://run.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fte.aibaodan.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oad.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rpn.ywan-chungtsiang.top

[N05] 最大公约数
来源：http://xlq.sysykeji.top

Py:   math.gcd(a, b)
来源：http://vbk.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ksn.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tjz.zhongyouzk.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qgv.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zhv.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jri.shangyingyoupin.top

Ruby: a.gcd(b)
来源：http://hfn.dashuyun.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wja.guowangkeji.top

[N06] 判断回文字符串
来源：http://hcu.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://bze.nanxinkj.top

PHP:  $s === strrev($s);
来源：http://abz.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://mpz.ctjpmb.com

TS:   s === [...s].reverse().join("")
来源：http://bjg.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://unm.yueranfly.top

Go:   // 双指针从两端比较
来源：http://cxd.gogol.net.cn

Ruby: s == s.reverse
来源：http://ycj.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rwe.smart0.xyz

[N07] 两数之和（返回下标）
来源：http://uwi.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://szs.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ofz.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://mni.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://cpe.jianghu66.top

Java: // 手写 HashMap
来源：http://nqu.dianchejie.cn

Go:   // 手写 map[int]int
来源：http://uao.sxryk.cn

Ruby: // 手写 Hash
来源：http://yku.zhiwuduotai.top

C#:   // 手写 Dictionary<int, int>
来源：http://kat.epnwcf.com

[N08] 生成全排列
来源：http://jsf.fehbvm.com

Py:   itertools.permutations(arr)
来源：http://wii.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://dwz.ivvv.top

JS:   // 手写回溯递归
来源：http://yxp.chenjidiqi.icu

TS:   // 手写回溯递归
来源：http://fzl.zhijiandao.cn

Java: // 手写回溯递归
来源：http://jfg.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://xpp.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://rqu.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://ztr.c1oappe.top

[N09] 栈与队列
来源：http://dto.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dpr.shanyushiyangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pjh.jinqigfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hce.sjlbkw.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pzv.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jkw.yj202588.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tgc.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lao.tarul.cn


<!-- 参考信息 -->