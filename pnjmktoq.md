代发 wailian999

[K06] 解析 URL 查询串
来源：http://qcz.sufxvd.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yjv.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ymu.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rny.ywan-chungtsiang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wcc.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bak.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qyl.hongshengwenyu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ywl.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vye.bjfxy.top

[K07] 进制转换
来源：http://vkm.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ofx.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xcz.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ult.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://aib.yangfankeji.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://unb.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tjc.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oof.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qqy.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://kir.yueranfly.top

Py:   pickle.dumps(obj)
来源：http://dud.hnxiangtu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://oke.cashguo.top

JS:   v8.serialize(obj)        // Node
来源：http://nlf.ivvv.top

TS:   v8.serialize(obj)        // Node
来源：http://adk.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gvo.zdbjq.cn

Go:   encoding/gob
来源：http://kiy.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://czt.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wgf.yfazqb.com

================================================================================
来源：http://cms.jinqigfzy.top

L. 网络请求
来源：http://cff.jqgfzy.top

================================================================================
来源：http://stq.ivvv.top

[L01] 发送 GET 请求
来源：http://adk.cqqwz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rku.fktsv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tan.pengpengdd.cyou

JS:   await fetch(url)
来源：http://osg.sxryk.cn

TS:   await fetch(url)
来源：http://rax.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ptv.tianlin.xyz

Go:   resp, err := http.Get(url)
来源：http://arz.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gzl.pengpengdd.cyou

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xbc.shzxlz.cn

[L02] 发送 POST JSON
来源：http://wga.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://zjz.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iqu.gaohongyu789.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vvs.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wcn.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://glg.feifeiyinyue.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://omv.gaohongyu789.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fxq.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xki.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://npq.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://inc.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jbm.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xcb.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ggg.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ycg.fehbvm.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://acj.hnqzz.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yrt.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lwn.cqqwz.cn

[L04] 设置超时
来源：http://gvk.fehbvm.com

Py:   requests.get(url, timeout=5)
来源：http://zvb.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ytl.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vkr.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hyg.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ilt.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sjp.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vmj.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gbc.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://efy.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vqo.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://phy.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iaz.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iry.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vaw.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kzd.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://acl.gogol.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zts.yvedp.cn

[L06] 解析响应为 JSON
来源：http://plu.hnxiangtu.top

Py:   resp.json()
来源：http://rqw.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://euw.hysaishi.cn

JS:   await resp.json()
来源：http://qip.daxiang520.top

TS:   await resp.json()
来源：http://ljg.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ldx.0kj1m.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hhr.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://sjx.zdqjudy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vga.sufxvd.cn

[L07] 处理 HTTP 状态码
来源：http://jzl.zhiwuduotai.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://thl.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vjz.meibo888.top

JS:   resp.ok;  resp.status
来源：http://poz.shanyushiyangkeji.top

TS:   resp.ok;  resp.status
来源：http://qei.guannengcc.top

Java: resp.statusCode()
来源：http://ddh.daxiang520.top

Go:   resp.StatusCode
来源：http://bdr.xziqi.cn

Ruby: resp.code.to_i
来源：http://pst.dianchejie.cn

C#:   (int)resp.StatusCode
来源：http://une.wangshuangyany.cn

[L08] 并发请求多个地址
来源：http://ykz.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xok.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://myd.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ckp.jyoumei.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yum.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wti.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pmo.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zwl.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://aat.zhengqikj.top

================================================================================
来源：http://mgl.meibo888.top

M. 命令行 / 进程 / 环境
来源：http://ogv.xingfuxueyuan.xyz

================================================================================
来源：http://mni.shanyushiyangtech.top

[M01] 读取命令行参数
来源：http://gle.yuanzhike.top

Py:   sys.argv[1:]
来源：http://dnf.ydzc1.top

PHP:  $argv;  $argc;
来源：http://ksq.hammf.cn

JS:   process.argv.slice(2)
来源：http://tbj.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://pab.xziqi.cn

Java: args 数组（main 方法参数）
来源：http://zpq.andypj.xyz

Go:   os.Args[1:]
来源：http://oih.ppjwa.cn

Ruby: ARGV
来源：http://kme.9152youxi.cn

C#:   args 数组（Main 方法参数）
来源：http://ahj.nanxinkj.top

[M02] 读取环境变量
来源：http://wvm.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://otb.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xkl.jiagoushi.top

JS:   process.env.HOME
来源：http://nbl.sufxvd.cn

TS:   process.env.HOME
来源：http://cji.epnwcf.com

Java: System.getenv("HOME")
来源：http://jcc.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qbu.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://jxg.c1oappe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kzn.jqgufenzy.top

[M03] 执行外部命令
来源：http://tuk.tianlin.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wfi.mhx1999.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://myq.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://uwe.feifeiyinyue.top

TS:   child_process.execSync("ls -l").toString()
来源：http://icw.cqqwz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://toz.tanke756.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xho.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wtl.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://apd.hnxiangtu.top

[M04] 获取当前工作目录
来源：http://iga.sjlbkw.cn

Py:   os.getcwd()
来源：http://srf.zhixingplan.top

PHP:  getcwd();
来源：http://cvo.sxryk.cn

JS:   process.cwd()
来源：http://toj.jqgufenzy.top

TS:   process.cwd()
来源：http://gaz.nanxuanxn.top

Java: Path.of("").toAbsolutePath()
来源：http://uvw.cucudq.cn

Go:   os.Getwd()
来源：http://yhb.guowangkeji.top

Ruby: Dir.pwd
来源：http://zcy.xingfuxueyuan.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ezt.yuanzhike.top

[M05] 设置退出码
来源：http://kuk.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://rvg.chenlongwang.top

PHP:  exit(1);
来源：http://wnl.zhongyouzk.top

JS:   process.exit(1)
来源：http://qet.9152youxi.cn

TS:   process.exit(1)
来源：http://dbj.ydjk.org.cn

Java: System.exit(1)
来源：http://uwy.cashguo.top

Go:   os.Exit(1)
来源：http://xex.epnwcf.com

Ruby: exit 1
来源：http://qlj.iojbl.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ezq.zycfv.cn

[M06] 向标准错误输出
来源：http://axc.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://hte.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://knk.zhixingplan.top

JS:   console.error("err")
来源：http://vlw.mhx1999.top

TS:   console.error("err")
来源：http://znl.zdqjudy.top

Java: System.err.println("err")
来源：http://ojs.yuxming.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wpp.yj20258.top

Ruby: warn "err"
来源：http://gko.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://blv.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://yln.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://wes.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aai.wangshuangyany.cn

JS:   require.main === module
来源：http://ncx.pengpengdd.cyou

TS:   require.main === module
来源：http://yjj.ctjpmb.com

Java: public static void main(String[] args)
来源：http://smu.guannengcc.top

Go:   func main()
来源：http://fqh.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tni.gzhubu.top

C#:   static void Main(string[] args)
来源：http://gvo.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://kys.hnxiangtu.top

Py:   platform.system();  platform.python_version()
来源：http://tvq.shanyushiyangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://ajq.gzhubu.top

JS:   process.platform;  process.version
来源：http://kqk.cheryme.top

TS:   process.platform;  process.version
来源：http://pql.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://swr.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mib.hammf.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qit.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vfg.dashuyun.cn

================================================================================
来源：http://tkn.gzhubu.top

N. 数据结构与算法
来源：http://ijk.xinyue.icu

================================================================================
来源：http://nhx.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://rcb.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://yxr.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vcn.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vth.zhoulong.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pob.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://vnq.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://pxc.shanyushiyangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zzf.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ske.zhengqikj.top

[N02] 排序（工程实践用内置实现）
来源：http://kqp.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://fvz.zhijiandao.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mrt.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://net.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ibo.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zuc.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://oyy.jinqigufen.top

Ruby: arr.sort
来源：http://vdn.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mux.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://jen.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://smr.yueranfly.top

PHP:  // 递归实现，或用 usort
来源：http://sjt.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://esu.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wjn.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://unn.uphjek.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jmy.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dtx.sjlbkw.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zvp.cucudq.cn

[N04] 斐波那契数列
来源：http://ece.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cvb.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kvl.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ioj.cucudq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ysa.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://smy.snrcjt.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lni.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://txz.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cge.yj202588.top

[N05] 最大公约数
来源：http://moo.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://afh.yj20258888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uzy.cucudq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cax.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tjf.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://luc.cqqwz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fxz.hfpthk.cn

Ruby: a.gcd(b)
来源：http://iqy.wangdashe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nbh.haohaochexian.top

[N06] 判断回文字符串
来源：http://qzu.ydzc1.top

Py:   s == s[::-1]
来源：http://jrk.hammf.cn

PHP:  $s === strrev($s);
来源：http://jhw.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://xvd.haohaochexian.top

TS:   s === [...s].reverse().join("")
来源：http://tjk.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dtc.aibaodan.cn

Go:   // 双指针从两端比较
来源：http://ofb.haohaochexian.top

Ruby: s == s.reverse
来源：http://wok.jianghu66.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rra.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://ocf.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xvu.chenzaomai.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mqp.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://yqn.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://ntp.316326.xyz

Java: // 手写 HashMap
来源：http://xux.zycfv.cn

Go:   // 手写 map[int]int
来源：http://osf.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://pct.zhixingplan.top

C#:   // 手写 Dictionary<int, int>
来源：http://axr.havefunace.top

[N08] 生成全排列
来源：http://uay.sweek.top

Py:   itertools.permutations(arr)
来源：http://lun.yonumen.top

PHP:  // 手写递归交换
来源：http://ibp.yonumen.top

JS:   // 手写回溯递归
来源：http://zam.gogol.net.cn

TS:   // 手写回溯递归
来源：http://bzo.daxiang520.top

Java: // 手写回溯递归
来源：http://jvk.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://zoe.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://tig.svipenyu.cn

C#:   // 手写回溯递归
来源：http://yni.yuxming.cn

[N09] 栈与队列
来源：http://ymq.ywan-chungtsiang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pcw.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hyr.tanke756.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xof.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ney.havefunace.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://exn.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mbc.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cjz.vqdsnc.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dfx.ydzc1.top

[N10] 链表节点定义
来源：http://rlf.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ufi.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://rrq.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yvh.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yun.zdbjq.cn

Java: class Node { int v; Node next; }
来源：http://zxz.pycfn.com

Go:   type Node struct { V int; Next *Node }
来源：http://hxe.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xbo.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hoz.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://fsj.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zfd.hywenlv.cn

PHP:  // 手写递归函数
来源：http://enk.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qde.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://chb.ydjk.org.cn

Java: // 手写递归
来源：http://uru.jyoumei.cn

Go:   // 手写递归
来源：http://qzj.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zhz.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://oky.zycfv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cbm.pycfn.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://npr.hywenlv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zbl.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lyc.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://udw.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mcd.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rmr.xuanzx.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hwb.ydjk.org.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fqo.ppjwa.cn

================================================================================
来源：http://azt.jinqigufen.top

O. 并发与异步
来源：http://qmz.dashuyun.cn

================================================================================
来源：http://min.zhijiandao.cn

[O01] 启动一个线程
来源：http://foj.cucudq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jbe.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jfc.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://niu.tanke756.top

TS:   // 同 JS
来源：http://rkb.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://mjt.yonumen.top

Go:   go f()
来源：http://vvj.zycfv.cn

Ruby: Thread.new { f }
来源：http://ldz.andypj.xyz

C#:   Task.Run(() => F());
来源：http://inx.xingfuxueyuan.xyz


<!-- 参考信息 -->