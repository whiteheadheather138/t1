代发 wailian999

TS:   JSON.parse(s)
来源：http://kuw.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uns.zdqjudy.top

Go:   json.Unmarshal(data, &v)
来源：http://yzx.redwolf501.top

Ruby: JSON.parse(s)
来源：http://hgq.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jlm.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://spt.ydjk.org.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pru.jyoumei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vvf.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://czh.9152youxi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xck.quarkkingdee.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://feb.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fln.zdbjq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dtn.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://akz.sweek.top

[K04] 读取 JSON 文件
来源：http://rjy.hongshengwenyu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bss.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://aiz.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ohw.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ejn.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ywm.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://riu.jinghuilouyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rwn.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hea.ydjk.org.cn

[K05] 深拷贝对象
来源：http://kdu.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://egy.gotoacloud.top

PHP:  unserialize(serialize($obj));
来源：http://ect.zhixingplan.top

JS:   structuredClone(obj)
来源：http://ygl.ctjpmb.com

TS:   structuredClone(obj)
来源：http://kik.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://omb.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ryn.yj20258.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wbw.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://upt.jlsjyb.cn

[K06] 解析 URL 查询串
来源：http://ofb.yangfankeji.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ewy.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xlq.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dop.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hxa.yongpay.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ynd.nanxuanxn.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mur.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fog.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wcq.zhiwuduotai.top

[K07] 进制转换
来源：http://tfj.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://faw.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eql.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://opp.ppjwa.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gmr.hongshengwenyu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zei.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bvm.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rpg.cheryme.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://drg.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://cux.ehwqpu.com

Py:   pickle.dumps(obj)
来源：http://aam.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dme.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://xpy.sxryk.cn

TS:   v8.serialize(obj)        // Node
来源：http://jnu.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://koo.andypj.xyz

Go:   encoding/gob
来源：http://kth.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://qyv.chenjidiqi.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://syq.sjlbkw.cn

================================================================================
来源：http://ejz.ppjwa.cn

L. 网络请求
来源：http://fto.jinqigfzy.top

================================================================================
来源：http://uqc.cheryme.top

[L01] 发送 GET 请求
来源：http://usn.vehdjk.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cnp.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://orn.andypj.xyz

JS:   await fetch(url)
来源：http://seo.shuidangran.top

TS:   await fetch(url)
来源：http://emr.jinghuilouyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cgm.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://dqj.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://hlk.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://euc.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://yuh.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uje.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://puy.bjfxy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hyf.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mqz.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qrh.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uec.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ljl.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eqi.shanyushiyangkeji.top

[L03] 设置自定义请求头
来源：http://vzy.yj20258.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hga.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kca.hongshengwenyu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ayb.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zpd.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gwm.guowangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zhr.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kfl.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lbp.316326.xyz

[L04] 设置超时
来源：http://sdx.yj20258888.top

Py:   requests.get(url, timeout=5)
来源：http://rtm.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ckw.guowangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gqj.ivvv.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qnt.cheryme.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sbr.zhixingplan.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ukl.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wmr.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ddu.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://azz.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://irx.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lfh.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xms.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fgi.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bcx.sufxvd.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fxe.snrcjt.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ile.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://esn.havefunace.top

[L06] 解析响应为 JSON
来源：http://zsk.jyoumei.cn

Py:   resp.json()
来源：http://wow.sweek.top

PHP:  json_decode($body, true);
来源：http://hka.xuetiantiany.cn

JS:   await resp.json()
来源：http://dhd.bjfxy.top

TS:   await resp.json()
来源：http://sbr.feifeiyinyue.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yci.xziqi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://plc.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://hli.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vvs.meibo888.top

[L07] 处理 HTTP 状态码
来源：http://ftd.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jzw.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vqe.yj202588.top

JS:   resp.ok;  resp.status
来源：http://peb.yongpay.top

TS:   resp.ok;  resp.status
来源：http://eja.yueranfly.top

Java: resp.statusCode()
来源：http://swy.yfazqb.com

Go:   resp.StatusCode
来源：http://ohg.dashuyun.cn

Ruby: resp.code.to_i
来源：http://tts.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://soz.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://jxg.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mbr.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://mcy.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hxk.zdqjudy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eho.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cbg.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cum.quarkkingdee.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rec.ydzc1.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yvy.jlsjyb.cn

================================================================================
来源：http://xxk.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://uwi.yvedp.cn

================================================================================
来源：http://yak.jqgfzy.top

[M01] 读取命令行参数
来源：http://dvt.52xcode.cn

Py:   sys.argv[1:]
来源：http://bcv.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://wss.sysykeji.top

JS:   process.argv.slice(2)
来源：http://mlr.gzhubu.top

TS:   process.argv.slice(2)
来源：http://lfu.smart0.xyz

Java: args 数组（main 方法参数）
来源：http://glm.wangdashe.top

Go:   os.Args[1:]
来源：http://iqj.gogol.net.cn

Ruby: ARGV
来源：http://mqr.cdnleiting.top

C#:   args 数组（Main 方法参数）
来源：http://xby.vehdjk.com

[M02] 读取环境变量
来源：http://kjc.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://kum.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mzz.hysaishi.cn

JS:   process.env.HOME
来源：http://qge.andypj.xyz

TS:   process.env.HOME
来源：http://gmw.tian-w.cn

Java: System.getenv("HOME")
来源：http://lpc.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wnd.smart0.xyz

Ruby: ENV["HOME"]
来源：http://qdd.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eeg.jqgufenzy.top

[M03] 执行外部命令
来源：http://hxx.andypj.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://plr.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ndb.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://crn.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://msd.fehbvm.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jjg.guowangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://elo.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://gcr.tian-w.cn

C#:   Process.Start("ls", "-l");
来源：http://swc.daria6918.cn

[M04] 获取当前工作目录
来源：http://pcb.hammf.cn

Py:   os.getcwd()
来源：http://xfg.yangfankeji.com

PHP:  getcwd();
来源：http://ktu.gzhubu.top

JS:   process.cwd()
来源：http://ima.ybcxt.top

TS:   process.cwd()
来源：http://rnl.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://hby.nanxinkj.top

Go:   os.Getwd()
来源：http://cij.hnqzz.top

Ruby: Dir.pwd
来源：http://hmt.zycfv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xmo.hysaishi.cn

[M05] 设置退出码
来源：http://ihy.gogol.net.cn

Py:   sys.exit(1)
来源：http://mkx.sjlbkw.cn

PHP:  exit(1);
来源：http://qab.kuanghao11.cn

JS:   process.exit(1)
来源：http://odt.jiagoushi.top

TS:   process.exit(1)
来源：http://snd.shangyingyoupin.top

Java: System.exit(1)
来源：http://hvl.0kj1m.cn

Go:   os.Exit(1)
来源：http://fsq.aizwys.cn

Ruby: exit 1
来源：http://osg.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bcj.aizwys.cn

[M06] 向标准错误输出
来源：http://jlu.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://syj.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://aut.yuanzhike.top

JS:   console.error("err")
来源：http://rhq.nanxuanxn.top

TS:   console.error("err")
来源：http://fzn.yuxming.cn

Java: System.err.println("err")
来源：http://wcj.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tgu.zhiwuduotai.top

Ruby: warn "err"
来源：http://xvn.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://wdi.xinyue.icu

[M07] 判断是否为主入口
来源：http://kqz.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://wvr.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kve.shanyushiyangkeji.top

JS:   require.main === module
来源：http://hwh.cucudq.cn

TS:   require.main === module
来源：http://boc.haohaochexian.top

Java: public static void main(String[] args)
来源：http://oil.nwbrower.top

Go:   func main()
来源：http://mhm.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kcz.zhaomingkeji.xyz

C#:   static void Main(string[] args)
来源：http://xjd.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://dma.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://uib.hcnkem.com

PHP:  PHP_OS;  phpversion();
来源：http://rsm.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://pfg.gogol.net.cn

TS:   process.platform;  process.version
来源：http://vwy.zdbjq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://amw.hfpthk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jul.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eal.bjfxy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ogf.ehwqpu.com

================================================================================
来源：http://oci.zhixingplan.top

N. 数据结构与算法
来源：http://iqz.havefunace.top

================================================================================
来源：http://glb.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://ose.pengpengdd.cyou

Py:   bisect.bisect_left(arr, x)
来源：http://uup.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wrp.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bxu.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://irl.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cgv.ppjwa.cn

Go:   sort.SearchInts(arr, x)
来源：http://wvc.yongpay.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://geu.aizwys.cn

C#:   Array.BinarySearch(arr, x)
来源：http://moa.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://pzv.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://jjk.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ncq.bjfxy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cbf.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fta.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jbn.wangdashe.top

Go:   slices.Sort(arr)
来源：http://ijn.gaohongyu789.top

Ruby: arr.sort
来源：http://lrw.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bji.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://xjp.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dbk.aizwys.cn

PHP:  // 递归实现，或用 usort
来源：http://kzn.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ygm.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xxc.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rrx.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kmj.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yct.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cpe.0kj1m.cn

[N04] 斐波那契数列
来源：http://qtr.guannengcc.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pno.cashguo.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://thz.ybcxt.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://flt.feifeiyinyue.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dif.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pwj.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ifm.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ciw.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ttu.yj20258.top

[N05] 最大公约数
来源：http://ksv.sweek.top

Py:   math.gcd(a, b)
来源：http://ode.yj20258888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nfk.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vjl.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vtt.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://omv.ppjwa.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hpl.fengsongda.top

Ruby: a.gcd(b)
来源：http://uxh.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kfw.aibaodan.cn

[N06] 判断回文字符串
来源：http://zaa.haohaochexian.top

Py:   s == s[::-1]
来源：http://zoa.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://bbe.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://rso.xziqi.cn

TS:   s === [...s].reverse().join("")
来源：http://kmn.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jad.zycfv.cn

Go:   // 双指针从两端比较
来源：http://nra.yj202588.top

Ruby: s == s.reverse
来源：http://pat.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kzd.yj202588.top

[N07] 两数之和（返回下标）
来源：http://ncp.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jzd.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uyk.hnqzz.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hgk.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://ypc.hnqzz.top

Java: // 手写 HashMap
来源：http://xcp.haohaochexian.top

Go:   // 手写 map[int]int
来源：http://uoj.chenzaomai.com

Ruby: // 手写 Hash
来源：http://emo.jianghu66.top

C#:   // 手写 Dictionary<int, int>
来源：http://kkh.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://dxx.nwbrower.top

Py:   itertools.permutations(arr)
来源：http://yvy.zdbjq.cn

PHP:  // 手写递归交换
来源：http://feg.tarul.cn

JS:   // 手写回溯递归
来源：http://gky.pycfn.com

TS:   // 手写回溯递归
来源：http://prm.ywan-chungtsiang.top

Java: // 手写回溯递归
来源：http://byu.ydzc1.top

Go:   // 手写回溯递归
来源：http://jkj.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://ptu.sxryk.cn

C#:   // 手写回溯递归
来源：http://mro.zdbjq.cn

[N09] 栈与队列
来源：http://sdf.yueranfly.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vxb.shanyushiyangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ujh.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dbp.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kzp.xinyue.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xrt.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://awa.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bkr.cheryme.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pny.sjlbkw.cn

[N10] 链表节点定义
来源：http://dyr.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dms.xinyue.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://due.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dof.birdmap.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ygv.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://zoj.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://sjd.svipenyu.cn


<!-- 参考信息 -->