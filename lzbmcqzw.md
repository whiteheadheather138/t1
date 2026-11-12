代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nnm.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aku.yuxming.cn

JS:   JSON.stringify(obj)
来源：http://cag.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://vru.guowangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jpx.xylfe.cn

Go:   json.Marshal(obj)
来源：http://nqz.jyoumei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ant.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://shk.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://edv.cdnleiting.top

Py:   json.loads(s)
来源：http://uzm.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gte.zycfv.cn

JS:   JSON.parse(s)
来源：http://ccn.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://xic.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://poz.sjlbkw.cn

Go:   json.Unmarshal(data, &v)
来源：http://eid.daxiang520.top

Ruby: JSON.parse(s)
来源：http://bof.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wfw.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://ttj.zhoulong.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cwj.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rkp.smart0.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://syo.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ctz.xylfe.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hgv.guowangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lnl.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://emp.svipenyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zev.pengpengdd.cyou

[K04] 读取 JSON 文件
来源：http://rsw.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://upp.meibo888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ajr.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://swc.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oca.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fmh.svipenyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bbl.jinghuilouyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hia.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zfb.aizwys.cn

[K05] 深拷贝对象
来源：http://bff.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://cac.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://hwv.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://dyu.ydjk.org.cn

TS:   structuredClone(obj)
来源：http://cnv.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://zdr.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mia.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mxh.xylfe.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ibf.chenlongwang.top

[K06] 解析 URL 查询串
来源：http://bgb.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lzy.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tyx.yueranfly.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qju.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wxy.zhixingplan.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uzm.ybcxt.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nlu.andypj.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mgd.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://das.bjfxy.top

[K07] 进制转换
来源：http://tro.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cit.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rwe.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zjr.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iyw.jlsjyb.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dyk.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://opj.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oxv.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ccn.hnxiangtu.top

[K08] 二进制序列化（非 JSON）
来源：http://yej.zdqjudy.top

Py:   pickle.dumps(obj)
来源：http://rgf.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dgn.chenlongwang.top

JS:   v8.serialize(obj)        // Node
来源：http://ajc.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://xfb.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uwz.fanxiaobao.xyz

Go:   encoding/gob
来源：http://ogu.zhixingplan.top

Ruby: Marshal.dump(obj)
来源：http://bka.zhoulong.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://myf.jinghuilouyu.cn

================================================================================
来源：http://yyj.fanxiaobao.xyz

L. 网络请求
来源：http://pha.zhixingplan.top

================================================================================
来源：http://ieu.tanke756.top

[L01] 发送 GET 请求
来源：http://nnp.ydjk.org.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lgz.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xor.xuanzx.com

JS:   await fetch(url)
来源：http://hhm.dashuyun.cn

TS:   await fetch(url)
来源：http://rxv.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gcn.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://mbg.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://plh.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ezo.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://hxr.52xcode.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hgv.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qef.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zbr.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vql.yonumen.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zwq.daria6918.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jzm.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jrs.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ioi.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://roj.ctjpmb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kwl.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fve.zdbjq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rmn.vqdsnc.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pur.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://clz.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mbb.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nbe.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iki.vqdsnc.cn

[L04] 设置超时
来源：http://arn.dashuyun.cn

Py:   requests.get(url, timeout=5)
来源：http://pgt.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ffz.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://duc.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hdy.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lxf.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kix.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eca.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://agl.cashguo.top

[L05] 上传文件（multipart）
来源：http://odm.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uxx.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vlu.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://usw.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://npk.meibo888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://auw.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tcu.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ose.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://unb.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://vye.jinqigufen.top

Py:   resp.json()
来源：http://ppv.nwbrower.top

PHP:  json_decode($body, true);
来源：http://zog.tanke756.top

JS:   await resp.json()
来源：http://tsi.guowangkeji.top

TS:   await resp.json()
来源：http://hrw.tanke756.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://upk.redwolf501.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lru.ydzc1.top

Ruby: JSON.parse(resp.body)
来源：http://dee.nwbrower.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://znk.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://yds.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ylx.yongpay.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lac.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://afw.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://boy.ctjpmb.com

Java: resp.statusCode()
来源：http://pou.hnqzz.top

Go:   resp.StatusCode
来源：http://otk.xziqi.cn

Ruby: resp.code.to_i
来源：http://ffj.cdnleiting.top

C#:   (int)resp.StatusCode
来源：http://hpj.uphjek.com

[L08] 并发请求多个地址
来源：http://guq.shanyushiyangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cvm.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://hfn.hfpthk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tiq.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ohg.cheryme.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tya.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fbf.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rod.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ntn.daria6918.cn

================================================================================
来源：http://qep.jinqigfzy.top

M. 命令行 / 进程 / 环境
来源：http://tpk.cheryme.top

================================================================================
来源：http://fgu.9152youxi.cn

[M01] 读取命令行参数
来源：http://jjw.shangyingyoupin.top

Py:   sys.argv[1:]
来源：http://iwf.andypj.xyz

PHP:  $argv;  $argc;
来源：http://ouk.yongpay.top

JS:   process.argv.slice(2)
来源：http://anp.fktsv.cn

TS:   process.argv.slice(2)
来源：http://res.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://jug.zycfv.cn

Go:   os.Args[1:]
来源：http://szh.jyoumei.cn

Ruby: ARGV
来源：http://hoa.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://ezz.hysaishi.cn

[M02] 读取环境变量
来源：http://tmy.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://rll.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pxq.chenlongwang.top

JS:   process.env.HOME
来源：http://awe.smart0.xyz

TS:   process.env.HOME
来源：http://uet.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://lkp.tanke756.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ipd.xuanzx.com

Ruby: ENV["HOME"]
来源：http://omn.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cbw.hammf.cn

[M03] 执行外部命令
来源：http://jst.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://spp.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jqt.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ysw.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pwe.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gmu.hywenlv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mvv.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://hrw.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://ocd.wangdashe.top

[M04] 获取当前工作目录
来源：http://ljt.vehdjk.com

Py:   os.getcwd()
来源：http://uvy.redwolf501.top

PHP:  getcwd();
来源：http://etj.wangshuangyany.cn

JS:   process.cwd()
来源：http://dnw.shuidangran.top

TS:   process.cwd()
来源：http://njo.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://ddj.redwolf501.top

Go:   os.Getwd()
来源：http://nsb.jqgfzy.top

Ruby: Dir.pwd
来源：http://brj.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://yqn.pengpengdd.cyou

[M05] 设置退出码
来源：http://jtf.kuanghao11.cn

Py:   sys.exit(1)
来源：http://xjc.shanyushiyangkeji.top

PHP:  exit(1);
来源：http://nil.tian-w.cn

JS:   process.exit(1)
来源：http://rwj.birdmap.top

TS:   process.exit(1)
来源：http://aam.zhiwuduotai.top

Java: System.exit(1)
来源：http://ukm.cheryme.top

Go:   os.Exit(1)
来源：http://eez.jianghu66.top

Ruby: exit 1
来源：http://eew.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hgu.gaohongyu789.top

[M06] 向标准错误输出
来源：http://fti.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://pev.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://evc.cheryme.top

JS:   console.error("err")
来源：http://cuu.zhiwuduotai.top

TS:   console.error("err")
来源：http://sva.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://zyz.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ucr.xuanzx.com

Ruby: warn "err"
来源：http://nie.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://ibp.jqgfzy.top

[M07] 判断是否为主入口
来源：http://tsx.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://ehf.xylfe.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zar.c1oappe.top

JS:   require.main === module
来源：http://qew.dashuyun.cn

TS:   require.main === module
来源：http://ncs.zhengqikj.top

Java: public static void main(String[] args)
来源：http://zqr.xingfuxueyuan.xyz

Go:   func main()
来源：http://ixw.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sak.tanke756.top

C#:   static void Main(string[] args)
来源：http://tua.hnxiangtu.top

[M08] 获取系统与运行时信息
来源：http://llf.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://fqd.wangshuangyany.cn

PHP:  PHP_OS;  phpversion();
来源：http://tyd.daxiang520.top

JS:   process.platform;  process.version
来源：http://kkh.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://ajm.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cvv.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qsv.xuanzx.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://unc.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jpu.dashuyun.cn

================================================================================
来源：http://rep.fktsv.cn

N. 数据结构与算法
来源：http://peq.gzhubu.top

================================================================================
来源：http://gqf.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://exu.gotoacloud.top

Py:   bisect.bisect_left(arr, x)
来源：http://lpb.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nxf.cucudq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pcw.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jhp.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://eol.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://ezu.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qrs.zhengqikj.top

C#:   Array.BinarySearch(arr, x)
来源：http://rmt.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://nrw.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://qcq.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ufj.52xcode.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cfd.nwbrower.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kad.quarkkingdee.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rlz.cheryme.top

Go:   slices.Sort(arr)
来源：http://wea.shuidangran.top

Ruby: arr.sort
来源：http://swg.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kaa.shanyushiyangtech.top

[N03] 快速排序（分治示例）
来源：http://qly.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ors.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://vkb.snrcjt.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hsv.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gkt.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://djb.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://atm.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rht.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vns.dashuyun.cn

[N04] 斐波那契数列
来源：http://hfm.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vdi.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cep.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cah.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hzr.svipenyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mtj.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gfc.jinghuilouyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sjb.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blq.wangshuangyany.cn

[N05] 最大公约数
来源：http://weo.fzhhl.top

Py:   math.gcd(a, b)
来源：http://qzh.gogol.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://svp.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uud.xziqi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://idg.svipenyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dat.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zgz.yongpay.top

Ruby: a.gcd(b)
来源：http://efg.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uxe.jqgfzy.top

[N06] 判断回文字符串
来源：http://zlo.uphjek.com

Py:   s == s[::-1]
来源：http://fzq.ydzc1.top

PHP:  $s === strrev($s);
来源：http://nbt.kuanghao11.cn

JS:   s === [...s].reverse().join("")
来源：http://ngq.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://ysb.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hgr.jinqigufen.top

Go:   // 双指针从两端比较
来源：http://puy.epnwcf.com

Ruby: s == s.reverse
来源：http://vxf.ywan-chungtsiang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://thr.jinqigufen.top

[N07] 两数之和（返回下标）
来源：http://gob.yuanzhike.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fhv.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://apz.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ybj.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://sxq.jiagoushi.top

Java: // 手写 HashMap
来源：http://jis.sxryk.cn

Go:   // 手写 map[int]int
来源：http://xgr.cucudq.cn

Ruby: // 手写 Hash
来源：http://xvu.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://rvp.hesvh.cn

[N08] 生成全排列
来源：http://qzl.pycfn.com

Py:   itertools.permutations(arr)
来源：http://blo.tian-w.cn

PHP:  // 手写递归交换
来源：http://ntn.dianchejie.cn

JS:   // 手写回溯递归
来源：http://bxo.ctjpmb.com

TS:   // 手写回溯递归
来源：http://hdg.9152youxi.cn

Java: // 手写回溯递归
来源：http://npt.zhoulong.xyz

Go:   // 手写回溯递归
来源：http://iab.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://fyq.mhx1999.top

C#:   // 手写回溯递归
来源：http://fjx.dashuyun.cn

[N09] 栈与队列
来源：http://zmz.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ibz.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gtc.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://whq.havefunace.top


<!-- 参考信息 -->