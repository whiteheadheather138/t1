代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pyp.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jbw.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://kvv.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://tls.epnwcf.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yyw.tarul.cn

Go:   json.Marshal(obj)
来源：http://yty.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://baa.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ifa.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://icb.daria6918.cn

Py:   json.loads(s)
来源：http://fzz.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vsr.guowangkeji.top

JS:   JSON.parse(s)
来源：http://fcc.ehwqpu.com

TS:   JSON.parse(s)
来源：http://eyu.xinyue.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wxo.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://srr.jlsjyb.cn

Ruby: JSON.parse(s)
来源：http://miq.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pwj.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://cia.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aba.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://luf.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pco.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ake.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vne.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wyq.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://sjc.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://osp.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://ute.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vvp.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rbs.ctjpmb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vuw.tian-w.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zmg.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oyj.cqqwz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zaf.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jdn.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cwm.tian-w.cn

[K05] 深拷贝对象
来源：http://yke.gogol.net.cn

Py:   copy.deepcopy(obj)
来源：http://mxg.zhoulong.xyz

PHP:  unserialize(serialize($obj));
来源：http://esh.guowangkeji.top

JS:   structuredClone(obj)
来源：http://wqn.cdnleiting.top

TS:   structuredClone(obj)
来源：http://ant.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sne.hnqzz.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sci.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://foa.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vdu.hammf.cn

[K06] 解析 URL 查询串
来源：http://wls.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://flz.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tnl.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gml.zhijiandao.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://akp.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hag.uphjek.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://sqv.ybcxt.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oxa.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dfc.yongpay.top

[K07] 进制转换
来源：http://jrw.vehdjk.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eze.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aek.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ial.pycfn.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tob.uphjek.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xxe.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lyx.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tlf.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wzh.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://ity.xuetiantiany.cn

Py:   pickle.dumps(obj)
来源：http://bmg.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://qlz.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://yyo.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://zcb.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ldv.nanxinkj.top

Go:   encoding/gob
来源：http://nlc.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://kaa.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://urh.nwbrower.top

================================================================================
来源：http://hoq.zhiwuduotai.top

L. 网络请求
来源：http://pxu.aizwys.cn

================================================================================
来源：http://zsm.shzxlz.cn

[L01] 发送 GET 请求
来源：http://vrl.yj20258888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sfu.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vwj.zhoulong.xyz

JS:   await fetch(url)
来源：http://bzg.snrcjt.cn

TS:   await fetch(url)
来源：http://mog.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yax.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://jdm.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fny.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gej.xziqi.cn

[L02] 发送 POST JSON
来源：http://xvy.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xqc.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lkm.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ehf.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sac.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rqa.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pmi.zycfv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://brv.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vjq.dianchejie.cn

[L03] 设置自定义请求头
来源：http://yya.chenjidiqi.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://abl.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mum.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hmy.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yny.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xua.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wqq.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tll.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ndd.fktsv.cn

[L04] 设置超时
来源：http://guw.bjfxy.top

Py:   requests.get(url, timeout=5)
来源：http://mvk.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pwz.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uww.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sup.316326.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pxt.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dxk.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://heu.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tsl.shuidangran.top

[L05] 上传文件（multipart）
来源：http://jth.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zwn.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ouq.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fbg.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://izf.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vti.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uuc.yongpay.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fya.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zer.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://vgf.nanxuanxn.top

Py:   resp.json()
来源：http://cfs.yongpay.top

PHP:  json_decode($body, true);
来源：http://hnv.zhongyouzk.top

JS:   await resp.json()
来源：http://pmm.aibaodan.cn

TS:   await resp.json()
来源：http://rca.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zcu.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ccr.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://rzg.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oow.jyoumei.cn

[L07] 处理 HTTP 状态码
来源：http://rrv.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xdb.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ona.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://rkk.52xcode.cn

TS:   resp.ok;  resp.status
来源：http://lcw.yueranfly.top

Java: resp.statusCode()
来源：http://nmf.sweek.top

Go:   resp.StatusCode
来源：http://njt.smart0.xyz

Ruby: resp.code.to_i
来源：http://kbq.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://rqx.hesvh.cn

[L08] 并发请求多个地址
来源：http://haz.zhixingplan.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bgj.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://ugi.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oev.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lfn.bbcook.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tat.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://not.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ldn.shanyushiyangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ths.gotoacloud.top

================================================================================
来源：http://pik.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://raq.daxiang520.top

================================================================================
来源：http://myj.vqdsnc.cn

[M01] 读取命令行参数
来源：http://phv.fehbvm.com

Py:   sys.argv[1:]
来源：http://axo.52xcode.cn

PHP:  $argv;  $argc;
来源：http://bgm.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://bcy.uphjek.com

TS:   process.argv.slice(2)
来源：http://ngh.ydzc1.top

Java: args 数组（main 方法参数）
来源：http://jrr.ivvv.top

Go:   os.Args[1:]
来源：http://jgs.zhengqikj.top

Ruby: ARGV
来源：http://mba.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://mub.yanxiufei.cn

[M02] 读取环境变量
来源：http://rxw.svipenyu.cn

Py:   os.environ.get("HOME")
来源：http://rny.vehdjk.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ipr.shangyingyoupin.top

JS:   process.env.HOME
来源：http://fpr.tarul.cn

TS:   process.env.HOME
来源：http://lct.tianlin.xyz

Java: System.getenv("HOME")
来源：http://zrd.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tkq.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://uzi.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://alh.uphjek.com

[M03] 执行外部命令
来源：http://pca.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fvh.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://foi.ybcxt.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wpn.dianchejie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gik.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iot.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wcb.meibo888.top

Ruby: system("ls -l");  `ls -l`
来源：http://qhi.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://gvf.epnwcf.com

[M04] 获取当前工作目录
来源：http://hhb.chenjidiqi.icu

Py:   os.getcwd()
来源：http://vrb.guowangkeji.top

PHP:  getcwd();
来源：http://laj.shangyingyoupin.top

JS:   process.cwd()
来源：http://gfx.shangyingyoupin.top

TS:   process.cwd()
来源：http://hfl.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://pxn.sufxvd.cn

Go:   os.Getwd()
来源：http://dji.xinyue.icu

Ruby: Dir.pwd
来源：http://rti.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://jov.shuidangran.top

[M05] 设置退出码
来源：http://ggk.gzhubu.top

Py:   sys.exit(1)
来源：http://wax.ydjk.org.cn

PHP:  exit(1);
来源：http://xgf.nanxinkj.top

JS:   process.exit(1)
来源：http://ljh.jinqigfzy.top

TS:   process.exit(1)
来源：http://bxe.vehdjk.com

Java: System.exit(1)
来源：http://fnn.yangfankeji.com

Go:   os.Exit(1)
来源：http://ftp.fanxiaobao.xyz

Ruby: exit 1
来源：http://zbp.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://swy.hcnkem.com

[M06] 向标准错误输出
来源：http://pdo.xingfuxueyuan.xyz

Py:   print("err", file=sys.stderr)
来源：http://zai.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://oby.yfazqb.com

JS:   console.error("err")
来源：http://vbv.zycfv.cn

TS:   console.error("err")
来源：http://zqx.jiagoushi.top

Java: System.err.println("err")
来源：http://lml.xuetiantiany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vnw.yuxming.cn

Ruby: warn "err"
来源：http://pfz.yvedp.cn

C#:   Console.Error.WriteLine("err")
来源：http://xgb.dianchejie.cn

[M07] 判断是否为主入口
来源：http://pmc.fehbvm.com

Py:   if __name__ == "__main__":
来源：http://tsh.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xlv.dashuyun.cn

JS:   require.main === module
来源：http://pwj.chenlongwang.top

TS:   require.main === module
来源：http://bsu.shuidangran.top

Java: public static void main(String[] args)
来源：http://kwz.xinyue.icu

Go:   func main()
来源：http://djk.hysaishi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://okj.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://vly.cucudq.cn

[M08] 获取系统与运行时信息
来源：http://lme.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://bae.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://jox.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://nyy.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://neo.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cow.ctjpmb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://fpl.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dvj.gzhubu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://icy.sysykeji.top

================================================================================
来源：http://quj.sufxvd.cn

N. 数据结构与算法
来源：http://vdc.wangdashe.top

================================================================================
来源：http://pfq.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://glm.dashuyun.cn

Py:   bisect.bisect_left(arr, x)
来源：http://abb.zdqjudy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://odu.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hxu.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uuq.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://tos.chenjidiqi.icu

Go:   sort.SearchInts(arr, x)
来源：http://byx.yj20258.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ige.jyoumei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lcs.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://fms.jiagoushi.top

Py:   sorted(arr);  arr.sort()
来源：http://orp.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qxd.ctjpmb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://eba.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hrv.cqqwz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hky.ydzc1.top

Go:   slices.Sort(arr)
来源：http://ono.cashguo.top

Ruby: arr.sort
来源：http://dqj.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vep.yongpay.top

[N03] 快速排序（分治示例）
来源：http://yej.yj20258.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dyn.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://oyb.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qty.snrcjt.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yds.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://haf.shangyingyoupin.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yky.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jmo.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://jxl.jyoumei.cn

[N04] 斐波那契数列
来源：http://hct.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pnk.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jdb.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ziw.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fsp.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://inw.jianghu66.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ipd.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tni.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tad.hammf.cn

[N05] 最大公约数
来源：http://ufk.xylfe.cn

Py:   math.gcd(a, b)
来源：http://ssx.fzhhl.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fhn.svipenyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jul.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rjq.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jmm.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xbe.chenlongwang.top

Ruby: a.gcd(b)
来源：http://kyk.ybcxt.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rag.sufxvd.cn

[N06] 判断回文字符串
来源：http://gym.ybcxt.top

Py:   s == s[::-1]
来源：http://gwi.wangdashe.top

PHP:  $s === strrev($s);
来源：http://onx.smart0.xyz

JS:   s === [...s].reverse().join("")
来源：http://fym.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://jwe.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mzz.aizwys.cn

Go:   // 双指针从两端比较
来源：http://rvl.hnxiangtu.top

Ruby: s == s.reverse
来源：http://cpu.smart0.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://pxa.zhixingplan.top

[N07] 两数之和（返回下标）
来源：http://tpd.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://brp.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hxe.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://lug.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://sbd.hammf.cn

Java: // 手写 HashMap
来源：http://off.hammf.cn

Go:   // 手写 map[int]int
来源：http://pdi.sjlbkw.cn

Ruby: // 手写 Hash
来源：http://tol.shanyushiyangtech.top

C#:   // 手写 Dictionary<int, int>
来源：http://syg.ydzc1.top

[N08] 生成全排列
来源：http://rqm.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://vay.yfazqb.com

PHP:  // 手写递归交换
来源：http://oev.daria6918.cn

JS:   // 手写回溯递归
来源：http://slw.xinyue.icu

TS:   // 手写回溯递归
来源：http://fbp.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://rup.gotoacloud.top

Go:   // 手写回溯递归
来源：http://ayz.ybcxt.top

Ruby: arr.permutation.to_a
来源：http://jbz.zycfv.cn

C#:   // 手写回溯递归
来源：http://iyz.gaohongyu789.top

[N09] 栈与队列
来源：http://niw.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gqf.guowangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kur.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ted.dashuyun.cn


<!-- 参考信息 -->