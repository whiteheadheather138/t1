代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://irf.kuanghao11.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nga.c1oappe.top

JS:   JSON.stringify(obj)
来源：http://rzk.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://wuu.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oob.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://hui.hnqzz.top

Ruby: obj.to_json                                     // require "json"
来源：http://dqk.yongpay.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cza.havefunace.top

[K02] JSON 字符串转对象
来源：http://yqg.hcnkem.com

Py:   json.loads(s)
来源：http://oen.yongpay.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ylc.nanxinkj.top

JS:   JSON.parse(s)
来源：http://hhg.shanyushiyangkeji.top

TS:   JSON.parse(s)
来源：http://xrf.316326.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xvz.kuanghao11.cn

Go:   json.Unmarshal(data, &v)
来源：http://gza.zdqjudy.top

Ruby: JSON.parse(s)
来源：http://eyu.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wof.tianlin.xyz

[K03] JSON 美化输出（带缩进）
来源：http://vkz.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sha.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pyi.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://noo.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rnx.shanyushiyangtech.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oli.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ggp.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://hec.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ros.fehbvm.com

[K04] 读取 JSON 文件
来源：http://fnp.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cku.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fvi.fzhhl.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hby.hnqzz.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zeb.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rew.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vwr.ivvv.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qyh.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kqe.sjlbkw.cn

[K05] 深拷贝对象
来源：http://tua.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://vfw.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://bey.fengsongda.top

JS:   structuredClone(obj)
来源：http://oel.yuxming.cn

TS:   structuredClone(obj)
来源：http://zkj.gogol.net.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rjp.wangshuangyany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yla.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nuo.epnwcf.com

C#:   // 序列化往返，或自定义 Clone
来源：http://lwn.gzhubu.top

[K06] 解析 URL 查询串
来源：http://zyt.yuxming.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cqu.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lkz.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fth.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fms.svipenyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.zhiwuduotai.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yna.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tfk.jinghuilouyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mdy.svipenyu.cn

[K07] 进制转换
来源：http://mwz.snrcjt.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cmr.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hrq.hnxiangtu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zhs.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vpb.yvedp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gwu.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uqc.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ryf.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pow.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://rcj.dianchejie.cn

Py:   pickle.dumps(obj)
来源：http://xzd.yongpay.top

PHP:  serialize($obj);  unserialize($s);
来源：http://kox.hnqzz.top

JS:   v8.serialize(obj)        // Node
来源：http://tmd.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://uwu.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uct.0kj1m.cn

Go:   encoding/gob
来源：http://awh.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://psf.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ucl.xuetiantiany.cn

================================================================================
来源：http://ykw.havefunace.top

L. 网络请求
来源：http://dku.vehdjk.com

================================================================================
来源：http://iyu.hysaishi.cn

[L01] 发送 GET 请求
来源：http://fdj.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wgk.jqgufenzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tzu.316326.xyz

JS:   await fetch(url)
来源：http://deh.nanxinkj.top

TS:   await fetch(url)
来源：http://wwu.wangdashe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xvp.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://ank.zhongyouzk.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jrk.mhx1999.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dey.0kj1m.cn

[L02] 发送 POST JSON
来源：http://itl.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://kvu.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sah.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aew.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ojm.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rac.andypj.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mgc.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kmx.bjfxy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://thn.zdqjudy.top

[L03] 设置自定义请求头
来源：http://fri.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vie.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wxd.hywenlv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vvj.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://htg.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qpa.yanxiufei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mzw.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://grr.wangshuangyany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://teo.redwolf501.top

[L04] 设置超时
来源：http://lzr.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://xix.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hut.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://chx.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qoq.tarul.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://idu.daria6918.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yck.jinqigufen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cad.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jfp.smart0.xyz

[L05] 上传文件（multipart）
来源：http://xfb.zhixingplan.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://obh.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fsn.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xxd.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ott.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mpy.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ybs.svipenyu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cre.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hhg.zhoulong.xyz

[L06] 解析响应为 JSON
来源：http://mmb.jqgufenzy.top

Py:   resp.json()
来源：http://drd.meibo888.top

PHP:  json_decode($body, true);
来源：http://exh.smart0.xyz

JS:   await resp.json()
来源：http://zhv.nwbrower.top

TS:   await resp.json()
来源：http://xuk.jqgfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://msb.0kj1m.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dqh.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://asy.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kxi.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://pkw.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://giv.chenlongwang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ken.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://eqz.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://guy.smart0.xyz

Java: resp.statusCode()
来源：http://rnu.jqgufenzy.top

Go:   resp.StatusCode
来源：http://eti.jqgfzy.top

Ruby: resp.code.to_i
来源：http://lcq.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://xck.aibaodan.cn

[L08] 并发请求多个地址
来源：http://eom.xylfe.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zwv.xuanzx.com

PHP:  curl_multi_init() 系列
来源：http://udr.andypj.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ccj.xylfe.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://adr.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kqk.pengpengdd.cyou

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eva.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ask.vqdsnc.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yxg.xinyue.icu

================================================================================
来源：http://wnh.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://dmy.yanxiufei.cn

================================================================================
来源：http://ntp.redwolf501.top

[M01] 读取命令行参数
来源：http://sqm.birdmap.top

Py:   sys.argv[1:]
来源：http://jon.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://lri.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://dkw.iojbl.cn

TS:   process.argv.slice(2)
来源：http://wod.sxryk.cn

Java: args 数组（main 方法参数）
来源：http://rbv.cheryme.top

Go:   os.Args[1:]
来源：http://kov.ehwqpu.com

Ruby: ARGV
来源：http://pbj.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://hfo.cdnleiting.top

[M02] 读取环境变量
来源：http://ovz.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://atq.zdqjudy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jgn.aibaodan.cn

JS:   process.env.HOME
来源：http://kqe.9152youxi.cn

TS:   process.env.HOME
来源：http://gue.cqqwz.cn

Java: System.getenv("HOME")
来源：http://pdw.svipenyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nbb.fzhhl.top

Ruby: ENV["HOME"]
来源：http://uzm.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qoc.hongshengwenyu.top

[M03] 执行外部命令
来源：http://jnu.yueranfly.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oen.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zcv.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://tlh.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ktg.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xia.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xsl.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://dbz.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://jsw.ctjpmb.com

[M04] 获取当前工作目录
来源：http://ypk.yj20258888.top

Py:   os.getcwd()
来源：http://ibr.chenzaomai.com

PHP:  getcwd();
来源：http://bdi.fengsongda.top

JS:   process.cwd()
来源：http://eoj.xylfe.cn

TS:   process.cwd()
来源：http://csd.ivvv.top

Java: Path.of("").toAbsolutePath()
来源：http://uxm.52xcode.cn

Go:   os.Getwd()
来源：http://jxa.snrcjt.cn

Ruby: Dir.pwd
来源：http://bqz.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://cfr.hysaishi.cn

[M05] 设置退出码
来源：http://zok.hywenlv.cn

Py:   sys.exit(1)
来源：http://fqf.ivvv.top

PHP:  exit(1);
来源：http://hqw.wangdashe.top

JS:   process.exit(1)
来源：http://yxe.fehbvm.com

TS:   process.exit(1)
来源：http://eou.mhx1999.top

Java: System.exit(1)
来源：http://wjn.sysykeji.top

Go:   os.Exit(1)
来源：http://ayj.jlsjyb.cn

Ruby: exit 1
来源：http://mkn.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://opo.zdbjq.cn

[M06] 向标准错误输出
来源：http://pvx.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://ihm.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vky.zdqjudy.top

JS:   console.error("err")
来源：http://sck.daria6918.cn

TS:   console.error("err")
来源：http://fin.hywenlv.cn

Java: System.err.println("err")
来源：http://uoa.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://brp.xinyue.icu

Ruby: warn "err"
来源：http://oiq.epnwcf.com

C#:   Console.Error.WriteLine("err")
来源：http://gbr.chenzaomai.com

[M07] 判断是否为主入口
来源：http://eej.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://brk.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dne.daxiang520.top

JS:   require.main === module
来源：http://zkf.fanxiaobao.xyz

TS:   require.main === module
来源：http://jag.yj20258888.top

Java: public static void main(String[] args)
来源：http://nbw.zhijiandao.cn

Go:   func main()
来源：http://czo.ydzc1.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://grw.zhongyouzk.top

C#:   static void Main(string[] args)
来源：http://mxq.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://flf.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://vak.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://lcg.vehdjk.com

JS:   process.platform;  process.version
来源：http://ruh.zdbjq.cn

TS:   process.platform;  process.version
来源：http://kgw.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zcx.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ded.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ivm.xingfuxueyuan.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://qgs.yfazqb.com

================================================================================
来源：http://xxw.jqgfzy.top

N. 数据结构与算法
来源：http://yne.fehbvm.com

================================================================================
来源：http://sjf.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://sap.aibaodan.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ejo.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vjc.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nex.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aoe.yvedp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bvl.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://hwp.jinyuanbaomall.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://otm.hammf.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aqp.cucudq.cn

[N02] 排序（工程实践用内置实现）
来源：http://rnz.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://zlu.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dud.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://erj.cdnleiting.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qwb.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yak.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://pkh.andypj.xyz

Ruby: arr.sort
来源：http://xiy.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tsb.xuanzx.com

[N03] 快速排序（分治示例）
来源：http://iib.chenzaomai.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ipe.hcnkem.com

PHP:  // 递归实现，或用 usort
来源：http://oob.nanxinkj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rdl.birdmap.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lvx.guowangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eam.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://let.ctjpmb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pfe.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://vkp.daxiang520.top

[N04] 斐波那契数列
来源：http://nkx.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ifc.zdqjudy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://thy.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lqi.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jzb.gaohongyu789.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pbc.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ani.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hgw.yanxiufei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://skg.zdbjq.cn

[N05] 最大公约数
来源：http://vbk.cashguo.top

Py:   math.gcd(a, b)
来源：http://zcg.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qkb.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://czr.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iuc.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sac.hnqzz.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cad.dianchejie.cn

Ruby: a.gcd(b)
来源：http://pxm.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fas.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://pjt.jinqigfzy.top

Py:   s == s[::-1]
来源：http://gak.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://ktr.zhixingplan.top

JS:   s === [...s].reverse().join("")
来源：http://hnh.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://gba.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mly.feifeiyinyue.top

Go:   // 双指针从两端比较
来源：http://woq.wangdashe.top

Ruby: s == s.reverse
来源：http://sfb.hcnkem.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://mfd.birdmap.top

[N07] 两数之和（返回下标）
来源：http://uqv.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fxw.tian-w.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iud.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vvy.jlsjyb.cn

TS:   // 手写 Map<string, number>
来源：http://ife.jlsjyb.cn

Java: // 手写 HashMap
来源：http://gcs.mhx1999.top

Go:   // 手写 map[int]int
来源：http://rqr.fehbvm.com

Ruby: // 手写 Hash
来源：http://xqr.cucudq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bpu.yfazqb.com

[N08] 生成全排列
来源：http://vxp.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://sgb.shanyushiyangkeji.top

PHP:  // 手写递归交换
来源：http://fvh.ehwqpu.com

JS:   // 手写回溯递归
来源：http://vxy.xinyue.icu

TS:   // 手写回溯递归
来源：http://ruv.yonumen.top

Java: // 手写回溯递归
来源：http://xnu.chenjidiqi.icu

Go:   // 手写回溯递归
来源：http://yyg.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://wmm.ydzc1.top

C#:   // 手写回溯递归
来源：http://nuz.hnqzz.top

[N09] 栈与队列
来源：http://eep.sxryk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pmu.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jke.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ubg.cashguo.top


<!-- 参考信息 -->