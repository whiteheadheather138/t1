代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ujs.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://klq.guowangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mzx.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qdy.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gaz.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wjx.guannengcc.top

[K08] 二进制序列化（非 JSON）
来源：http://exl.dashuyun.cn

Py:   pickle.dumps(obj)
来源：http://bwn.shangyingyoupin.top

PHP:  serialize($obj);  unserialize($s);
来源：http://oow.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://rig.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://dlo.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vvz.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://yzj.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://ils.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iys.fengsongda.top

================================================================================
来源：http://vox.yj202588.top

L. 网络请求
来源：http://eme.bjfxy.top

================================================================================
来源：http://rld.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://olb.tian-w.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xfj.zhiwuduotai.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zvu.sxryk.cn

JS:   await fetch(url)
来源：http://aqv.havefunace.top

TS:   await fetch(url)
来源：http://udl.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nwx.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://vou.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uqa.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sxi.shuidangran.top

[L02] 发送 POST JSON
来源：http://rae.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://khm.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tad.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qqz.fktsv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wrh.dianchejie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cfy.hammf.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tlu.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ydo.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://egl.guannengcc.top

[L03] 设置自定义请求头
来源：http://dtf.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rme.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rkg.dashuyun.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fzq.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uys.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gmi.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jel.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rjz.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sqq.chenlongwang.top

[L04] 设置超时
来源：http://xtg.xuetiantiany.cn

Py:   requests.get(url, timeout=5)
来源：http://cjp.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fpx.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://olh.yonumen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wlf.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pfg.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jqb.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ebo.wangdashe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jjs.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://fxv.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vly.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gyb.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nza.kuanghao11.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dkw.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tis.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ead.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vyy.chenzaomai.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rqh.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://hpt.quarkkingdee.top

Py:   resp.json()
来源：http://fes.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://hbl.0kj1m.cn

JS:   await resp.json()
来源：http://cdj.dianchejie.cn

TS:   await resp.json()
来源：http://zda.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jar.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kni.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://cou.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mwa.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://rps.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fah.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://htd.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://oey.yuanzhike.top

TS:   resp.ok;  resp.status
来源：http://pyl.0kj1m.cn

Java: resp.statusCode()
来源：http://pgr.yongpay.top

Go:   resp.StatusCode
来源：http://egb.hysaishi.cn

Ruby: resp.code.to_i
来源：http://lzo.cashguo.top

C#:   (int)resp.StatusCode
来源：http://wwp.mhx1999.top

[L08] 并发请求多个地址
来源：http://kel.hesvh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kip.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://unr.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vsu.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kkk.vehdjk.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xji.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zvg.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lec.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fbl.jqgufenzy.top

================================================================================
来源：http://trq.hongshengwenyu.top

M. 命令行 / 进程 / 环境
来源：http://bbr.shanyushiyangkeji.top

================================================================================
来源：http://zst.daria6918.cn

[M01] 读取命令行参数
来源：http://fyu.chenzaomai.com

Py:   sys.argv[1:]
来源：http://jah.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://fex.sweek.top

JS:   process.argv.slice(2)
来源：http://rqh.xingfuxueyuan.xyz

TS:   process.argv.slice(2)
来源：http://ugb.shanyushiyangkeji.top

Java: args 数组（main 方法参数）
来源：http://xwe.yonumen.top

Go:   os.Args[1:]
来源：http://tly.yueranfly.top

Ruby: ARGV
来源：http://bho.dashuyun.cn

C#:   args 数组（Main 方法参数）
来源：http://pxj.xylfe.cn

[M02] 读取环境变量
来源：http://oxm.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://kbu.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yba.fengsongda.top

JS:   process.env.HOME
来源：http://thi.andypj.xyz

TS:   process.env.HOME
来源：http://bax.yuxming.cn

Java: System.getenv("HOME")
来源：http://qiq.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://thz.jqgufenzy.top

Ruby: ENV["HOME"]
来源：http://qpn.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://svz.zhixingplan.top

[M03] 执行外部命令
来源：http://que.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mku.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fdu.shangyingyoupin.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ftt.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qve.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jkn.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://taf.52xcode.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bdc.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://izs.fktsv.cn

[M04] 获取当前工作目录
来源：http://cvf.yj20258.top

Py:   os.getcwd()
来源：http://pqj.fanxiaobao.xyz

PHP:  getcwd();
来源：http://eot.zdbjq.cn

JS:   process.cwd()
来源：http://oir.hesvh.cn

TS:   process.cwd()
来源：http://sas.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://ttr.nwbrower.top

Go:   os.Getwd()
来源：http://kbu.kuanghao11.cn

Ruby: Dir.pwd
来源：http://dlu.zhixingplan.top

C#:   Directory.GetCurrentDirectory()
来源：http://pfp.redwolf501.top

[M05] 设置退出码
来源：http://zkp.iojbl.cn

Py:   sys.exit(1)
来源：http://uvv.iojbl.cn

PHP:  exit(1);
来源：http://mbz.jqgfzy.top

JS:   process.exit(1)
来源：http://dvf.jianghu66.top

TS:   process.exit(1)
来源：http://glq.jlsjyb.cn

Java: System.exit(1)
来源：http://tci.hfpthk.cn

Go:   os.Exit(1)
来源：http://ojk.guannengcc.top

Ruby: exit 1
来源：http://aca.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cbw.shuidangran.top

[M06] 向标准错误输出
来源：http://wdu.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://fnb.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wje.cucudq.cn

JS:   console.error("err")
来源：http://ssl.sufxvd.cn

TS:   console.error("err")
来源：http://sma.jinqigfzy.top

Java: System.err.println("err")
来源：http://pla.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rzd.zdbjq.cn

Ruby: warn "err"
来源：http://yhi.yj202588.top

C#:   Console.Error.WriteLine("err")
来源：http://twc.cucudq.cn

[M07] 判断是否为主入口
来源：http://mzj.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://kdf.tarul.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zki.yj202588.top

JS:   require.main === module
来源：http://poh.iojbl.cn

TS:   require.main === module
来源：http://dla.shzxlz.cn

Java: public static void main(String[] args)
来源：http://phk.havefunace.top

Go:   func main()
来源：http://nzu.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lud.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://fmy.chenzaomai.com

[M08] 获取系统与运行时信息
来源：http://gqk.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://aqp.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://eyv.xinyue.icu

JS:   process.platform;  process.version
来源：http://tde.guannengcc.top

TS:   process.platform;  process.version
来源：http://csi.sjlbkw.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ukj.xinyue.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://wtm.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ypi.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fjd.xuanzx.com

================================================================================
来源：http://uju.daria6918.cn

N. 数据结构与算法
来源：http://ypo.nwbrower.top

================================================================================
来源：http://ozg.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://slw.zhiwuduotai.top

Py:   bisect.bisect_left(arr, x)
来源：http://wmn.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hxf.dianchejie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tel.wangshuangyany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oup.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://rcg.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://krz.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sip.daria6918.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qen.jianghu66.top

[N02] 排序（工程实践用内置实现）
来源：http://zie.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://bqr.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zcg.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mzh.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://okf.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://reb.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://tgz.iojbl.cn

Ruby: arr.sort
来源：http://eeq.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rdo.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://bqs.smart0.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vev.wangshuangyany.cn

PHP:  // 递归实现，或用 usort
来源：http://weh.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jms.gotoacloud.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kvg.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oxk.ydzc1.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vyu.jinghuilouyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kkp.ivvv.top

C#:   // 手写递归，或 Array.Sort
来源：http://dys.mhx1999.top

[N04] 斐波那契数列
来源：http://naw.vehdjk.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xuz.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://clx.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hcd.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ggu.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zqe.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vxm.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://duy.ydjk.org.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wgs.fehbvm.com

[N05] 最大公约数
来源：http://fif.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://kub.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bij.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vds.redwolf501.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yqq.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://grr.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tpi.nanxuanxn.top

Ruby: a.gcd(b)
来源：http://bth.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lgw.daxiang520.top

[N06] 判断回文字符串
来源：http://vxx.snrcjt.cn

Py:   s == s[::-1]
来源：http://tze.yvedp.cn

PHP:  $s === strrev($s);
来源：http://suc.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://scv.havefunace.top

TS:   s === [...s].reverse().join("")
来源：http://kac.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hob.hesvh.cn

Go:   // 双指针从两端比较
来源：http://fpn.zhengqikj.top

Ruby: s == s.reverse
来源：http://isz.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://oai.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://qhs.yuanzhike.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wup.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lsy.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mha.ydzc1.top

TS:   // 手写 Map<string, number>
来源：http://oxs.zycfv.cn

Java: // 手写 HashMap
来源：http://xfb.bjfxy.top

Go:   // 手写 map[int]int
来源：http://bje.wangdashe.top

Ruby: // 手写 Hash
来源：http://qle.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://qyv.nanxuanxn.top

[N08] 生成全排列
来源：http://fem.52xcode.cn

Py:   itertools.permutations(arr)
来源：http://vjt.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://rts.hammf.cn

JS:   // 手写回溯递归
来源：http://qxs.52xcode.cn

TS:   // 手写回溯递归
来源：http://hpk.ppjwa.cn

Java: // 手写回溯递归
来源：http://ryt.yuxming.cn

Go:   // 手写回溯递归
来源：http://joc.sjlbkw.cn

Ruby: arr.permutation.to_a
来源：http://bka.andypj.xyz

C#:   // 手写回溯递归
来源：http://aze.gogol.net.cn

[N09] 栈与队列
来源：http://qmb.guannengcc.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://izn.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://apu.dianchejie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vjf.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rir.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cpf.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dju.jinyuanbaomall.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gfj.chenjidiqi.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zba.hcnkem.com

[N10] 链表节点定义
来源：http://qos.zhongyouzk.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://khb.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aff.0kj1m.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qnm.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oqc.aibaodan.cn

Java: class Node { int v; Node next; }
来源：http://dgv.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://nos.shanyushiyangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mec.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://guh.zhiwuduotai.top

[N11] 二叉树中序遍历
来源：http://aeu.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qsd.hammf.cn

PHP:  // 手写递归函数
来源：http://jhn.daria6918.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://spl.nanxinkj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ypz.shuidangran.top

Java: // 手写递归
来源：http://fia.c1oappe.top

Go:   // 手写递归
来源：http://huu.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nog.zhijiandao.cn

C#:   // 手写递归
来源：http://qdb.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://esv.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sqi.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fzb.jiagoushi.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://phr.gotoacloud.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aaq.ctjpmb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mjt.shanyushiyangtech.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qxg.daria6918.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tpe.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mgv.gzhubu.top

================================================================================
来源：http://syr.sufxvd.cn

O. 并发与异步
来源：http://qrm.pengpengdd.cyou

================================================================================
来源：http://asx.jqgufenzy.top

[O01] 启动一个线程
来源：http://zhq.gzhubu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nwm.c1oappe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qzz.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ieo.jinqigfzy.top

TS:   // 同 JS
来源：http://qny.wangdashe.top

Java: new Thread(() -> f()).start()
来源：http://spo.svipenyu.cn

Go:   go f()
来源：http://fyd.sysykeji.top

Ruby: Thread.new { f }
来源：http://lid.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://fpb.quarkkingdee.top

[O02] 使用线程池
来源：http://vxb.kuanghao11.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zyw.cashguo.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xsz.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://edd.gaohongyu789.top

TS:   // worker_threads 线程池
来源：http://tpg.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://jnp.ydzc1.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jqz.shuidangran.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vbl.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lsx.c1oappe.top

[O03] 加锁保护共享数据
来源：http://wkz.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://rvl.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://yrc.fehbvm.com


<!-- 参考信息 -->