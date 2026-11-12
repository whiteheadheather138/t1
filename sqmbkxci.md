代发 wailian999

[K02] JSON 字符串转对象
来源：http://icf.jinqigufen.top

Py:   json.loads(s)
来源：http://btj.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vsi.yj202588.top

JS:   JSON.parse(s)
来源：http://dqz.gogol.net.cn

TS:   JSON.parse(s)
来源：http://fmi.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rhr.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://igx.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://wij.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://viv.vehdjk.com

[K03] JSON 美化输出（带缩进）
来源：http://ikd.epnwcf.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://psx.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qyh.yfazqb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://tpw.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xxe.hongshengwenyu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ngy.hysaishi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bas.birdmap.top

Ruby: JSON.pretty_generate(obj)
来源：http://vfv.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://use.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://xpo.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zsx.zhijiandao.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xkv.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lra.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wsj.hywenlv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lhr.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dwu.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ojj.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lse.vqdsnc.cn

[K05] 深拷贝对象
来源：http://oug.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://uzv.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://jbq.nanxinkj.top

JS:   structuredClone(obj)
来源：http://xtm.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://zjt.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uqx.hammf.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://esd.zhaomingkeji.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://emo.316326.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ifm.dianchejie.cn

[K06] 解析 URL 查询串
来源：http://lib.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wfw.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lsd.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pxi.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lxb.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tiu.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yxj.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ttg.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ode.yueranfly.top

[K07] 进制转换
来源：http://doc.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ahj.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bge.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tqx.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uec.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://isn.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://byq.havefunace.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ykm.yvedp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blk.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://hpd.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://rns.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ffc.nanxinkj.top

JS:   v8.serialize(obj)        // Node
来源：http://fux.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://eui.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bli.zdbjq.cn

Go:   encoding/gob
来源：http://ezr.hongshengwenyu.top

Ruby: Marshal.dump(obj)
来源：http://lye.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jcz.hnxiangtu.top

================================================================================
来源：http://srl.guannengcc.top

L. 网络请求
来源：http://fga.tanke756.top

================================================================================
来源：http://bws.aizwys.cn

[L01] 发送 GET 请求
来源：http://kis.zdbjq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oqo.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iih.jyoumei.cn

JS:   await fetch(url)
来源：http://uxz.zhongyouzk.top

TS:   await fetch(url)
来源：http://dga.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uir.iojbl.cn

Go:   resp, err := http.Get(url)
来源：http://zxn.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zny.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ctl.jinyuanbaomall.cn

[L02] 发送 POST JSON
来源：http://chg.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://oli.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qoy.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qmh.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://umf.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rrr.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tag.cheryme.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ght.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ruz.ywan-chungtsiang.top

[L03] 设置自定义请求头
来源：http://plt.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wrq.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://znc.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xbp.52xcode.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wzn.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://csy.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yww.iojbl.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ebf.xinyue.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sat.ydzc1.top

[L04] 设置超时
来源：http://clz.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://fxx.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mev.ydzc1.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ibz.vehdjk.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yyg.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fyo.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vgd.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tby.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ylu.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://rdq.nwbrower.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tnt.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://raa.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rhg.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mbk.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://twb.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mlo.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hrm.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://srk.shuidangran.top

[L06] 解析响应为 JSON
来源：http://wet.jinqigfzy.top

Py:   resp.json()
来源：http://hcv.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://mng.jlsjyb.cn

JS:   await resp.json()
来源：http://cgv.tian-w.cn

TS:   await resp.json()
来源：http://rch.smart0.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jax.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nki.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://vrm.cheryme.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://txy.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://ese.meibo888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uuc.xinyue.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://unx.gotoacloud.top

JS:   resp.ok;  resp.status
来源：http://gee.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://swh.wangdashe.top

Java: resp.statusCode()
来源：http://dek.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://kol.fehbvm.com

Ruby: resp.code.to_i
来源：http://ssu.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://mor.birdmap.top

[L08] 并发请求多个地址
来源：http://kqd.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jlt.zhongyouzk.top

PHP:  curl_multi_init() 系列
来源：http://ysm.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://odl.zdqjudy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lxw.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hol.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ysx.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oqk.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hgd.zdqjudy.top

================================================================================
来源：http://iqq.yueranfly.top

M. 命令行 / 进程 / 环境
来源：http://mzi.0kj1m.cn

================================================================================
来源：http://yjd.hfpthk.cn

[M01] 读取命令行参数
来源：http://hqv.hongshengwenyu.top

Py:   sys.argv[1:]
来源：http://vat.xuanzx.com

PHP:  $argv;  $argc;
来源：http://ogn.nanxinkj.top

JS:   process.argv.slice(2)
来源：http://jsu.yfazqb.com

TS:   process.argv.slice(2)
来源：http://eal.zhengqikj.top

Java: args 数组（main 方法参数）
来源：http://idz.epnwcf.com

Go:   os.Args[1:]
来源：http://qnm.hcnkem.com

Ruby: ARGV
来源：http://yey.pengpengdd.cyou

C#:   args 数组（Main 方法参数）
来源：http://jjd.xuetiantiany.cn

[M02] 读取环境变量
来源：http://gck.birdmap.top

Py:   os.environ.get("HOME")
来源：http://kwo.fanxiaobao.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jjo.c1oappe.top

JS:   process.env.HOME
来源：http://rof.ywan-chungtsiang.top

TS:   process.env.HOME
来源：http://lhn.yuanzhike.top

Java: System.getenv("HOME")
来源：http://zql.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wrr.nwbrower.top

Ruby: ENV["HOME"]
来源：http://ivy.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jpm.tanke756.top

[M03] 执行外部命令
来源：http://rxw.birdmap.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tko.smart0.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vnh.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cku.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://evs.ehwqpu.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fxy.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dwp.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ecw.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://mzn.yongpay.top

[M04] 获取当前工作目录
来源：http://aoi.epnwcf.com

Py:   os.getcwd()
来源：http://nda.fehbvm.com

PHP:  getcwd();
来源：http://kwv.shzxlz.cn

JS:   process.cwd()
来源：http://mxi.guannengcc.top

TS:   process.cwd()
来源：http://aaf.ctjpmb.com

Java: Path.of("").toAbsolutePath()
来源：http://jnb.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://baj.sysykeji.top

Ruby: Dir.pwd
来源：http://ojf.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://fyn.fehbvm.com

[M05] 设置退出码
来源：http://elh.andypj.xyz

Py:   sys.exit(1)
来源：http://jze.jlsjyb.cn

PHP:  exit(1);
来源：http://tmw.yj20258.top

JS:   process.exit(1)
来源：http://nvs.gogol.net.cn

TS:   process.exit(1)
来源：http://ufg.jianghu66.top

Java: System.exit(1)
来源：http://tnk.meibo888.top

Go:   os.Exit(1)
来源：http://hrj.yj20258.top

Ruby: exit 1
来源：http://oje.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://efr.ybcxt.top

[M06] 向标准错误输出
来源：http://fch.shanyushiyangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://izi.wangdashe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://thm.yvedp.cn

JS:   console.error("err")
来源：http://rqn.hnxiangtu.top

TS:   console.error("err")
来源：http://pof.dianchejie.cn

Java: System.err.println("err")
来源：http://adl.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wpn.svipenyu.cn

Ruby: warn "err"
来源：http://ngw.bjfxy.top

C#:   Console.Error.WriteLine("err")
来源：http://ooc.meibo888.top

[M07] 判断是否为主入口
来源：http://nqw.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://tkb.xylfe.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qnx.svipenyu.cn

JS:   require.main === module
来源：http://zft.tianlin.xyz

TS:   require.main === module
来源：http://kgd.gogol.net.cn

Java: public static void main(String[] args)
来源：http://mni.pycfn.com

Go:   func main()
来源：http://qui.sjlbkw.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://frs.meibo888.top

C#:   static void Main(string[] args)
来源：http://lzq.vqdsnc.cn

[M08] 获取系统与运行时信息
来源：http://stk.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://xph.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://bpg.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://bfw.shzxlz.cn

TS:   process.platform;  process.version
来源：http://mgc.52xcode.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kjr.hywenlv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://aba.yanxiufei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kio.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://npb.zhaomingkeji.xyz

================================================================================
来源：http://mby.fengsongda.top

N. 数据结构与算法
来源：http://rks.xuetiantiany.cn

================================================================================
来源：http://ujh.52xcode.cn

[N01] 二分查找（有序数组）
来源：http://tyy.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yyu.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ndo.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nyy.9152youxi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://paw.52xcode.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nmv.jqgufenzy.top

Go:   sort.SearchInts(arr, x)
来源：http://skv.hywenlv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qow.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cfs.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://jzt.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://nvp.yueranfly.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bjx.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nve.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xri.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oas.snrcjt.cn

Go:   slices.Sort(arr)
来源：http://myr.yangfankeji.com

Ruby: arr.sort
来源：http://dqw.chenzaomai.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://bfc.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://alt.jinqigufen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://slk.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://xfu.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hsb.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hwv.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://abt.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mwn.xziqi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://alo.shzxlz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sqr.wangdashe.top

[N04] 斐波那契数列
来源：http://pjj.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ldk.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jfm.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gki.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hyg.tianlin.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jdw.sysykeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://keh.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aaf.wangshuangyany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ute.vqdsnc.cn

[N05] 最大公约数
来源：http://tck.fzhhl.top

Py:   math.gcd(a, b)
来源：http://ofc.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oue.jyoumei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jvh.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fxe.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lul.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://szp.andypj.xyz

Ruby: a.gcd(b)
来源：http://nvh.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://omf.zhongyouzk.top

[N06] 判断回文字符串
来源：http://kjb.hongshengwenyu.top

Py:   s == s[::-1]
来源：http://keo.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://teg.jianghu66.top

JS:   s === [...s].reverse().join("")
来源：http://esp.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://snj.sxryk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zwh.hongshengwenyu.top

Go:   // 双指针从两端比较
来源：http://qqr.yvedp.cn

Ruby: s == s.reverse
来源：http://bpr.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cvy.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://obj.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mze.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qpv.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rao.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://coh.cheryme.top

Java: // 手写 HashMap
来源：http://aww.nwbrower.top

Go:   // 手写 map[int]int
来源：http://now.xziqi.cn

Ruby: // 手写 Hash
来源：http://nck.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://ibq.meibo888.top

[N08] 生成全排列
来源：http://spv.pengpengdd.cyou

Py:   itertools.permutations(arr)
来源：http://fva.ivvv.top

PHP:  // 手写递归交换
来源：http://vyz.ybcxt.top

JS:   // 手写回溯递归
来源：http://cxc.ppjwa.cn

TS:   // 手写回溯递归
来源：http://wtx.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://xcm.sweek.top

Go:   // 手写回溯递归
来源：http://onf.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://tod.fzhhl.top

C#:   // 手写回溯递归
来源：http://vdk.jinghuilouyu.cn

[N09] 栈与队列
来源：http://oul.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iwt.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tpz.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oex.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qqs.fengsongda.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kgp.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://har.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nxj.yfazqb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://atc.aizwys.cn

[N10] 链表节点定义
来源：http://soq.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hvp.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://yaf.ybcxt.top


<!-- 参考信息 -->