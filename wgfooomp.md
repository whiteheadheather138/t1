代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eep.aizwys.cn

[K03] JSON 美化输出（带缩进）
来源：http://sli.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uwg.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yec.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kag.sjlbkw.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xgn.zhongyouzk.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dyw.fzhhl.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zey.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lhp.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iei.ppjwa.cn

[K04] 读取 JSON 文件
来源：http://uwm.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://asu.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://evz.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://awm.zdbjq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://twt.yj20258.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aau.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xsf.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mtp.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://whr.fktsv.cn

[K05] 深拷贝对象
来源：http://esf.shanyushiyangtech.top

Py:   copy.deepcopy(obj)
来源：http://hgm.bjfxy.top

PHP:  unserialize(serialize($obj));
来源：http://los.epnwcf.com

JS:   structuredClone(obj)
来源：http://oou.tarul.cn

TS:   structuredClone(obj)
来源：http://vqo.bbcook.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://kzw.hammf.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ybg.ppjwa.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xpv.nanxuanxn.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tyh.zdbjq.cn

[K06] 解析 URL 查询串
来源：http://cok.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yag.xylfe.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rqb.jqgufenzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lrg.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rtn.tarul.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ztb.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://raz.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cxj.52xcode.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hlh.kuanghao11.cn

[K07] 进制转换
来源：http://ule.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qif.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ooq.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jaq.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jry.cashguo.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zcv.hnqzz.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://exz.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zue.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yls.shuidangran.top

[K08] 二进制序列化（非 JSON）
来源：http://acg.sysykeji.top

Py:   pickle.dumps(obj)
来源：http://aeu.ydzc1.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gjg.dashuyun.cn

JS:   v8.serialize(obj)        // Node
来源：http://nue.gzhubu.top

TS:   v8.serialize(obj)        // Node
来源：http://pzk.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ntl.birdmap.top

Go:   encoding/gob
来源：http://ivb.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://fjw.shzxlz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wtk.cheryme.top

================================================================================
来源：http://agv.yfazqb.com

L. 网络请求
来源：http://qsr.yongpay.top

================================================================================
来源：http://aja.52xcode.cn

[L01] 发送 GET 请求
来源：http://odk.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wlq.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pda.ctjpmb.com

JS:   await fetch(url)
来源：http://myr.iojbl.cn

TS:   await fetch(url)
来源：http://znq.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mwq.yuxming.cn

Go:   resp, err := http.Get(url)
来源：http://wae.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wkm.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tnt.shanyushiyangkeji.top

[L02] 发送 POST JSON
来源：http://jyl.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://oux.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vyl.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wgd.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yub.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xua.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mps.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qen.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uhp.iojbl.cn

[L03] 设置自定义请求头
来源：http://gea.hongshengwenyu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jvb.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://txk.hfpthk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gjb.yj20258.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yvx.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bik.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mci.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://phj.xuetiantiany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dsi.pengpengdd.cyou

[L04] 设置超时
来源：http://ybi.yj20258.top

Py:   requests.get(url, timeout=5)
来源：http://iao.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hdx.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ddu.jqgufenzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lhg.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dnb.nwbrower.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fii.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://brh.xziqi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wic.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://mmk.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kzy.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ehw.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://npc.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yqq.yueranfly.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mad.ybcxt.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cng.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nrc.iojbl.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hxa.jianghu66.top

[L06] 解析响应为 JSON
来源：http://hrc.jqgfzy.top

Py:   resp.json()
来源：http://uon.fanxiaobao.xyz

PHP:  json_decode($body, true);
来源：http://gfm.chenjidiqi.icu

JS:   await resp.json()
来源：http://edu.zhengqikj.top

TS:   await resp.json()
来源：http://xge.meibo888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gwr.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ozl.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://aiz.epnwcf.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mqr.quarkkingdee.top

[L07] 处理 HTTP 状态码
来源：http://kbo.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://grh.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://riq.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://zqr.meibo888.top

TS:   resp.ok;  resp.status
来源：http://ync.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://tfu.shuidangran.top

Go:   resp.StatusCode
来源：http://txa.dashuyun.cn

Ruby: resp.code.to_i
来源：http://vol.snrcjt.cn

C#:   (int)resp.StatusCode
来源：http://ayk.tanke756.top

[L08] 并发请求多个地址
来源：http://fjb.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ujn.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://thg.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rfv.fengsongda.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ijc.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lom.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jxf.fzhhl.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mdx.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://irn.yfazqb.com

================================================================================
来源：http://qkd.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://ktz.ehwqpu.com

================================================================================
来源：http://eqz.52xcode.cn

[M01] 读取命令行参数
来源：http://kur.ehwqpu.com

Py:   sys.argv[1:]
来源：http://krh.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://myw.daria6918.cn

JS:   process.argv.slice(2)
来源：http://rtm.jlsjyb.cn

TS:   process.argv.slice(2)
来源：http://ure.xziqi.cn

Java: args 数组（main 方法参数）
来源：http://nvd.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://rud.jinqigfzy.top

Ruby: ARGV
来源：http://zqb.hammf.cn

C#:   args 数组（Main 方法参数）
来源：http://ctb.jianghu66.top

[M02] 读取环境变量
来源：http://urd.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://yzh.zdqjudy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tzk.zhoulong.xyz

JS:   process.env.HOME
来源：http://pej.kuanghao11.cn

TS:   process.env.HOME
来源：http://dku.zdqjudy.top

Java: System.getenv("HOME")
来源：http://ztl.feifeiyinyue.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oqi.redwolf501.top

Ruby: ENV["HOME"]
来源：http://efy.cqqwz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oxq.smart0.xyz

[M03] 执行外部命令
来源：http://jry.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lci.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dzu.c1oappe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ixb.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gko.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lob.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://spz.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://goe.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://asw.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://xgr.jiagoushi.top

Py:   os.getcwd()
来源：http://vfg.andypj.xyz

PHP:  getcwd();
来源：http://oqu.nanxinkj.top

JS:   process.cwd()
来源：http://pul.c1oappe.top

TS:   process.cwd()
来源：http://dgr.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://xgh.dianchejie.cn

Go:   os.Getwd()
来源：http://xnj.vehdjk.com

Ruby: Dir.pwd
来源：http://vsx.kuanghao11.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kbj.ydzc1.top

[M05] 设置退出码
来源：http://waj.ydzc1.top

Py:   sys.exit(1)
来源：http://vyi.yangfankeji.com

PHP:  exit(1);
来源：http://ejs.yuanzhike.top

JS:   process.exit(1)
来源：http://qxd.ydzc1.top

TS:   process.exit(1)
来源：http://ygv.svipenyu.cn

Java: System.exit(1)
来源：http://ezp.sweek.top

Go:   os.Exit(1)
来源：http://faf.zhengqikj.top

Ruby: exit 1
来源：http://njm.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yzu.xuanzx.com

[M06] 向标准错误输出
来源：http://zji.9152youxi.cn

Py:   print("err", file=sys.stderr)
来源：http://epj.epnwcf.com

PHP:  fwrite(STDERR, "err\n");
来源：http://cox.chenjidiqi.icu

JS:   console.error("err")
来源：http://lrd.cucudq.cn

TS:   console.error("err")
来源：http://gay.jiagoushi.top

Java: System.err.println("err")
来源：http://ozy.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sig.yj20258.top

Ruby: warn "err"
来源：http://dcd.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://cym.hnqzz.top

[M07] 判断是否为主入口
来源：http://kpc.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://lzo.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pbf.wangshuangyany.cn

JS:   require.main === module
来源：http://byw.jyoumei.cn

TS:   require.main === module
来源：http://hqm.fengsongda.top

Java: public static void main(String[] args)
来源：http://kkr.zdqjudy.top

Go:   func main()
来源：http://paa.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fed.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://uoe.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://pgj.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://bfg.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://jrc.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://ahv.cucudq.cn

TS:   process.platform;  process.version
来源：http://dxr.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cjk.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ksb.pycfn.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hnb.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qxl.ctjpmb.com

================================================================================
来源：http://mfx.wangdashe.top

N. 数据结构与算法
来源：http://ies.xylfe.cn

================================================================================
来源：http://ara.cheryme.top

[N01] 二分查找（有序数组）
来源：http://aen.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gbu.ctjpmb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eya.zhongyouzk.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kjb.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uko.dianchejie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xfq.jqgufenzy.top

Go:   sort.SearchInts(arr, x)
来源：http://gtr.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://her.epnwcf.com

C#:   Array.BinarySearch(arr, x)
来源：http://aig.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://inx.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://tka.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://djn.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pps.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qvz.hcnkem.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aqy.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://zyq.cucudq.cn

Ruby: arr.sort
来源：http://gby.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lta.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://jql.zhoulong.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://plv.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://ttg.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uqb.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ttg.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ofw.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pwb.9152youxi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://giw.hesvh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wwp.tianlin.xyz

[N04] 斐波那契数列
来源：http://uvp.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://azl.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rcr.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xtu.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ysw.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mag.hywenlv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sza.hesvh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fnt.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jqb.yj20258888.top

[N05] 最大公约数
来源：http://jcu.yonumen.top

Py:   math.gcd(a, b)
来源：http://nin.shangyingyoupin.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tqk.hesvh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://huv.yuxming.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wpt.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bxt.yueranfly.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hwe.wangdashe.top

Ruby: a.gcd(b)
来源：http://iig.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lyj.jiagoushi.top

[N06] 判断回文字符串
来源：http://gbf.yuanzhike.top

Py:   s == s[::-1]
来源：http://jli.jyoumei.cn

PHP:  $s === strrev($s);
来源：http://cip.sweek.top

JS:   s === [...s].reverse().join("")
来源：http://udq.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://jjx.ywan-chungtsiang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jfo.xuanzx.com

Go:   // 双指针从两端比较
来源：http://ppe.fengsongda.top

Ruby: s == s.reverse
来源：http://wqd.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bkh.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://chg.zhongyouzk.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://huq.cashguo.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ddo.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://uvx.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://uye.hnxiangtu.top

Java: // 手写 HashMap
来源：http://wjw.haohaochexian.top

Go:   // 手写 map[int]int
来源：http://fce.hnxiangtu.top

Ruby: // 手写 Hash
来源：http://qtf.fzhhl.top

C#:   // 手写 Dictionary<int, int>
来源：http://crd.hnqzz.top

[N08] 生成全排列
来源：http://ijp.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://kpu.andypj.xyz

PHP:  // 手写递归交换
来源：http://hys.mhx1999.top

JS:   // 手写回溯递归
来源：http://huz.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://knx.cqqwz.cn

Java: // 手写回溯递归
来源：http://nfd.sysykeji.top

Go:   // 手写回溯递归
来源：http://krz.aizwys.cn

Ruby: arr.permutation.to_a
来源：http://phm.ehwqpu.com

C#:   // 手写回溯递归
来源：http://ptr.smart0.xyz

[N09] 栈与队列
来源：http://pay.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vbn.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cff.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gfk.yangfankeji.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jfv.jlsjyb.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tnn.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oda.sjlbkw.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rak.yuanzhike.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wkx.fktsv.cn

[N10] 链表节点定义
来源：http://pex.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://evx.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://uwh.wangshuangyany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://okf.yueranfly.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ytr.gaohongyu789.top

Java: class Node { int v; Node next; }
来源：http://lxb.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wbi.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://cye.ydjk.org.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pnp.xinyue.icu

[N11] 二叉树中序遍历
来源：http://zjg.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bfr.gogol.net.cn


<!-- 参考信息 -->