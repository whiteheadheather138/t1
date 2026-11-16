代发 wailian999

================================================================================
来源：http://nim.yvedp.cn

K. JSON 与序列化
来源：http://gpw.zhaomingkeji.xyz

================================================================================
来源：http://xdc.cheryme.top

[K01] 对象转 JSON 字符串
来源：http://xzx.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jks.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nye.cqqwz.cn

JS:   JSON.stringify(obj)
来源：http://jcq.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://huj.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ugo.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://mef.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://cpk.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xff.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://acq.ehwqpu.com

Py:   json.loads(s)
来源：http://ysj.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lfj.ybcxt.top

JS:   JSON.parse(s)
来源：http://rrp.cheryme.top

TS:   JSON.parse(s)
来源：http://qdz.guannengcc.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wfq.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://yrw.yj202588.top

Ruby: JSON.parse(s)
来源：http://ntk.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yrl.jinyuanbaomall.cn

[K03] JSON 美化输出（带缩进）
来源：http://ciy.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nfy.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pek.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gdd.fehbvm.com

TS:   JSON.stringify(obj, null, 2)
来源：http://tgh.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wgh.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wec.kuanghao11.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ymc.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ear.gaohongyu789.top

[K04] 读取 JSON 文件
来源：http://atk.ppjwa.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aqv.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aqk.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pgm.sysykeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yay.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lhv.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tji.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nma.havefunace.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cjd.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://alj.feifeiyinyue.top

Py:   copy.deepcopy(obj)
来源：http://gps.0kj1m.cn

PHP:  unserialize(serialize($obj));
来源：http://fvm.fktsv.cn

JS:   structuredClone(obj)
来源：http://ndz.aizwys.cn

TS:   structuredClone(obj)
来源：http://kcq.shanyushiyangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://com.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kpg.aizwys.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jmd.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pav.nanxinkj.top

[K06] 解析 URL 查询串
来源：http://jxo.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uoz.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wov.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lqd.ivvv.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uwb.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sgv.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://nfl.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oyz.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zjd.vqdsnc.cn

[K07] 进制转换
来源：http://ftq.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jqq.kuanghao11.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jhm.9152youxi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gzb.mhx1999.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gbn.yj20258.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ovk.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qsv.jqgfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qwo.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oec.sjlbkw.cn

[K08] 二进制序列化（非 JSON）
来源：http://esv.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://xkr.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fjd.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://ncf.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://cgp.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sql.yuanzhike.top

Go:   encoding/gob
来源：http://ztm.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://ijj.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://icp.cqqwz.cn

================================================================================
来源：http://liy.yongpay.top

L. 网络请求
来源：http://hsh.smart0.xyz

================================================================================
来源：http://kqt.aibaodan.cn

[L01] 发送 GET 请求
来源：http://xgc.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gbj.yueranfly.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://drf.xuetiantiany.cn

JS:   await fetch(url)
来源：http://nso.fzhhl.top

TS:   await fetch(url)
来源：http://tef.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fdv.nwbrower.top

Go:   resp, err := http.Get(url)
来源：http://dzf.feifeiyinyue.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dao.tian-w.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uam.ydzc1.top

[L02] 发送 POST JSON
来源：http://xkg.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rhd.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://svd.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yng.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lrh.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://swc.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://llg.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://orc.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tcs.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://nck.guannengcc.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kvk.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jge.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ueg.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zqa.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qtg.smart0.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lzy.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qqt.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ntr.ivvv.top

[L04] 设置超时
来源：http://xgm.shzxlz.cn

Py:   requests.get(url, timeout=5)
来源：http://lkn.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rtn.jyoumei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://afw.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dvb.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://icr.cheryme.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wfc.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gxc.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kbh.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://tuj.feifeiyinyue.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jqw.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pkb.0kj1m.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mda.jianghu66.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ikh.birdmap.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ldk.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kqq.c1oappe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dxi.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rwv.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://wpa.chenlongwang.top

Py:   resp.json()
来源：http://job.wangshuangyany.cn

PHP:  json_decode($body, true);
来源：http://vjj.jinghuilouyu.cn

JS:   await resp.json()
来源：http://ybh.meibo888.top

TS:   await resp.json()
来源：http://apd.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zpw.shzxlz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ojn.xylfe.cn

Ruby: JSON.parse(resp.body)
来源：http://vux.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://npb.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://len.quarkkingdee.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://igi.fehbvm.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vgq.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://gla.jyoumei.cn

TS:   resp.ok;  resp.status
来源：http://hso.yuxming.cn

Java: resp.statusCode()
来源：http://ele.xinyue.icu

Go:   resp.StatusCode
来源：http://wah.tarul.cn

Ruby: resp.code.to_i
来源：http://ifn.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://ati.sysykeji.top

[L08] 并发请求多个地址
来源：http://agz.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://itw.hnxiangtu.top

PHP:  curl_multi_init() 系列
来源：http://rdm.dashuyun.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ret.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tee.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://liu.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rto.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hgp.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gpz.cheryme.top

================================================================================
来源：http://wfg.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://tfs.zhongyouzk.top

================================================================================
来源：http://cmp.jqgfzy.top

[M01] 读取命令行参数
来源：http://ojc.cucudq.cn

Py:   sys.argv[1:]
来源：http://hot.tanke756.top

PHP:  $argv;  $argc;
来源：http://hym.ehwqpu.com

JS:   process.argv.slice(2)
来源：http://chq.gzhubu.top

TS:   process.argv.slice(2)
来源：http://zvt.epnwcf.com

Java: args 数组（main 方法参数）
来源：http://ftn.cheryme.top

Go:   os.Args[1:]
来源：http://xvz.cashguo.top

Ruby: ARGV
来源：http://qbp.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://oex.chenjidiqi.icu

[M02] 读取环境变量
来源：http://mnm.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://hdi.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://drz.jlsjyb.cn

JS:   process.env.HOME
来源：http://ppt.smart0.xyz

TS:   process.env.HOME
来源：http://jip.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://tmj.mhx1999.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yzl.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://xnd.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wwg.hcnkem.com

[M03] 执行外部命令
来源：http://exo.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jhl.xingfuxueyuan.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fpi.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lko.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zet.zhongyouzk.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mhk.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ynn.cqqwz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qgi.pycfn.com

C#:   Process.Start("ls", "-l");
来源：http://yac.hcnkem.com

[M04] 获取当前工作目录
来源：http://gwk.yj20258.top

Py:   os.getcwd()
来源：http://bzy.0kj1m.cn

PHP:  getcwd();
来源：http://efi.yuxming.cn

JS:   process.cwd()
来源：http://wva.xziqi.cn

TS:   process.cwd()
来源：http://jko.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://ldr.ybcxt.top

Go:   os.Getwd()
来源：http://ieo.xylfe.cn

Ruby: Dir.pwd
来源：http://eca.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nih.yfazqb.com

[M05] 设置退出码
来源：http://cto.aibaodan.cn

Py:   sys.exit(1)
来源：http://ceu.andypj.xyz

PHP:  exit(1);
来源：http://ssb.nwbrower.top

JS:   process.exit(1)
来源：http://vyy.ydjk.org.cn

TS:   process.exit(1)
来源：http://lrc.sxryk.cn

Java: System.exit(1)
来源：http://zqa.snrcjt.cn

Go:   os.Exit(1)
来源：http://xvj.bbcook.cn

Ruby: exit 1
来源：http://kym.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gam.nanxuanxn.top

[M06] 向标准错误输出
来源：http://hpb.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://wls.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://igj.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://gny.yj202588.top

TS:   console.error("err")
来源：http://tun.cucudq.cn

Java: System.err.println("err")
来源：http://ylz.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://enb.9152youxi.cn

Ruby: warn "err"
来源：http://ojd.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://ahp.ppjwa.cn

[M07] 判断是否为主入口
来源：http://yjf.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://pzm.shanyushiyangtech.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jng.jinqigufen.top

JS:   require.main === module
来源：http://ukq.nanxinkj.top

TS:   require.main === module
来源：http://hfw.zdbjq.cn

Java: public static void main(String[] args)
来源：http://dtz.yuxming.cn

Go:   func main()
来源：http://elb.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xuw.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://drw.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://oxo.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://iyo.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://sfu.bjfxy.top

JS:   process.platform;  process.version
来源：http://mwe.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://fvr.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vxe.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qwf.pycfn.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fts.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ojv.jlsjyb.cn

================================================================================
来源：http://yca.shuidangran.top

N. 数据结构与算法
来源：http://xmk.daxiang520.top

================================================================================
来源：http://esm.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://wny.shangyingyoupin.top

Py:   bisect.bisect_left(arr, x)
来源：http://jtf.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eoh.birdmap.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uxx.tianlin.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ajr.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://ofb.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://ywl.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ttb.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://btv.xuanzx.com

[N02] 排序（工程实践用内置实现）
来源：http://pao.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://uil.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hfd.nanxuanxn.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vfk.zhiwuduotai.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fjn.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kyv.316326.xyz

Go:   slices.Sort(arr)
来源：http://fmb.yj202588.top

Ruby: arr.sort
来源：http://poo.xinyue.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://vsm.yvedp.cn

[N03] 快速排序（分治示例）
来源：http://twd.cdnleiting.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ouw.wangshuangyany.cn

PHP:  // 递归实现，或用 usort
来源：http://dqa.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cqc.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fic.guowangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nru.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://epw.jinyuanbaomall.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://whs.ywan-chungtsiang.top

C#:   // 手写递归，或 Array.Sort
来源：http://bwy.ydjk.org.cn

[N04] 斐波那契数列
来源：http://wkm.yueranfly.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ayp.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sbx.9152youxi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gkd.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vhc.wangshuangyany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tzi.jqgufenzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lci.nanxinkj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hqs.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wpo.ctjpmb.com

[N05] 最大公约数
来源：http://aly.hesvh.cn

Py:   math.gcd(a, b)
来源：http://axs.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fth.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sps.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jqr.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uta.jinqigfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://taw.redwolf501.top

Ruby: a.gcd(b)
来源：http://esn.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bdd.yuanzhike.top

[N06] 判断回文字符串
来源：http://zvx.chenjidiqi.icu

Py:   s == s[::-1]
来源：http://ypb.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://suw.uphjek.com

JS:   s === [...s].reverse().join("")
来源：http://xke.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://ata.xinyue.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dym.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://oxx.cashguo.top

Ruby: s == s.reverse
来源：http://mfe.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ovl.hcnkem.com

[N07] 两数之和（返回下标）
来源：http://zar.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ilk.jiagoushi.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ues.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mlb.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://ldj.aizwys.cn

Java: // 手写 HashMap
来源：http://xhy.dianchejie.cn

Go:   // 手写 map[int]int
来源：http://ooa.ppjwa.cn

Ruby: // 手写 Hash
来源：http://fpk.wangshuangyany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://var.dashuyun.cn

[N08] 生成全排列
来源：http://bbc.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://zpf.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://wwd.daria6918.cn

JS:   // 手写回溯递归
来源：http://gfx.sxryk.cn

TS:   // 手写回溯递归
来源：http://kfk.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://cif.epnwcf.com

Go:   // 手写回溯递归
来源：http://sii.meibo888.top

Ruby: arr.permutation.to_a
来源：http://bcr.ctjpmb.com

C#:   // 手写回溯递归
来源：http://ysv.c1oappe.top


<!-- 参考信息 -->