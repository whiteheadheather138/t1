代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iwv.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://org.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://mnd.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://knt.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://jpu.epnwcf.com

JS:   v8.serialize(obj)        // Node
来源：http://knz.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://gve.fzhhl.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bja.yongpay.top

Go:   encoding/gob
来源：http://cwv.cashguo.top

Ruby: Marshal.dump(obj)
来源：http://rwe.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://axu.ybcxt.top

================================================================================
来源：http://sdw.mhx1999.top

L. 网络请求
来源：http://ppg.andypj.xyz

================================================================================
来源：http://ejx.aibaodan.cn

[L01] 发送 GET 请求
来源：http://lnv.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ety.xylfe.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ddy.jinyuanbaomall.cn

JS:   await fetch(url)
来源：http://evn.yuxming.cn

TS:   await fetch(url)
来源：http://ztc.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yuj.zhongyouzk.top

Go:   resp, err := http.Get(url)
来源：http://fhm.guowangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rbi.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nhv.cucudq.cn

[L02] 发送 POST JSON
来源：http://vjo.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://vwt.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ssm.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jvg.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rlz.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://psf.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lbc.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tot.hnxiangtu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kha.shzxlz.cn

[L03] 设置自定义请求头
来源：http://zpe.yj202588.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cwz.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rji.jinqigfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pfm.fzhhl.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xio.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fre.yanxiufei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cjw.yfazqb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://azn.pycfn.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dla.jinyuanbaomall.cn

[L04] 设置超时
来源：http://atk.hnqzz.top

Py:   requests.get(url, timeout=5)
来源：http://ohp.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yjm.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lmt.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kqh.redwolf501.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tdb.yuanzhike.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pgt.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iva.zhijiandao.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hda.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://dwv.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jxa.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uhz.yvedp.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://htp.vehdjk.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sqx.sweek.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bgk.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://azo.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qgm.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wpg.xziqi.cn

[L06] 解析响应为 JSON
来源：http://wzb.nanxuanxn.top

Py:   resp.json()
来源：http://izu.pycfn.com

PHP:  json_decode($body, true);
来源：http://mom.gogol.net.cn

JS:   await resp.json()
来源：http://mob.shuidangran.top

TS:   await resp.json()
来源：http://zyj.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yly.guannengcc.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jnp.ydzc1.top

Ruby: JSON.parse(resp.body)
来源：http://pmd.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://alk.sjlbkw.cn

[L07] 处理 HTTP 状态码
来源：http://bpe.xuanzx.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mcg.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qfo.quarkkingdee.top

JS:   resp.ok;  resp.status
来源：http://ldn.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://bsj.chenlongwang.top

Java: resp.statusCode()
来源：http://wwy.cashguo.top

Go:   resp.StatusCode
来源：http://tek.ehwqpu.com

Ruby: resp.code.to_i
来源：http://jed.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://wkp.aibaodan.cn

[L08] 并发请求多个地址
来源：http://kyt.mhx1999.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ghd.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://ckb.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bfo.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xel.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ohc.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nok.hnxiangtu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://msp.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jtt.nanxinkj.top

================================================================================
来源：http://hry.yj20258888.top

M. 命令行 / 进程 / 环境
来源：http://vbc.jianghu66.top

================================================================================
来源：http://rof.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://oxq.sxryk.cn

Py:   sys.argv[1:]
来源：http://oqx.fengsongda.top

PHP:  $argv;  $argc;
来源：http://uoh.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://cbv.jlsjyb.cn

TS:   process.argv.slice(2)
来源：http://spw.hcnkem.com

Java: args 数组（main 方法参数）
来源：http://whp.ivvv.top

Go:   os.Args[1:]
来源：http://maf.guowangkeji.top

Ruby: ARGV
来源：http://twx.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://dbg.pengpengdd.cyou

[M02] 读取环境变量
来源：http://oqn.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://nmz.zdqjudy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xxl.yj20258888.top

JS:   process.env.HOME
来源：http://gzw.zhongyouzk.top

TS:   process.env.HOME
来源：http://edr.fengsongda.top

Java: System.getenv("HOME")
来源：http://ryl.cqqwz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sdc.hnxiangtu.top

Ruby: ENV["HOME"]
来源：http://onb.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://joa.fktsv.cn

[M03] 执行外部命令
来源：http://ltd.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wmo.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ybh.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fer.jlsjyb.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oxo.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gtt.xinyue.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://chk.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://taw.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://xno.hnqzz.top

[M04] 获取当前工作目录
来源：http://hii.feifeiyinyue.top

Py:   os.getcwd()
来源：http://yvb.pengpengdd.cyou

PHP:  getcwd();
来源：http://osu.yj202588.top

JS:   process.cwd()
来源：http://xja.bjfxy.top

TS:   process.cwd()
来源：http://ipl.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://nqd.yuanzhike.top

Go:   os.Getwd()
来源：http://com.birdmap.top

Ruby: Dir.pwd
来源：http://nam.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://yge.jlsjyb.cn

[M05] 设置退出码
来源：http://fvv.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://imk.chenjidiqi.icu

PHP:  exit(1);
来源：http://pdt.yangfankeji.com

JS:   process.exit(1)
来源：http://jhy.yangfankeji.com

TS:   process.exit(1)
来源：http://fbc.cheryme.top

Java: System.exit(1)
来源：http://krn.ydjk.org.cn

Go:   os.Exit(1)
来源：http://jio.wangdashe.top

Ruby: exit 1
来源：http://pyd.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://paz.chenlongwang.top

[M06] 向标准错误输出
来源：http://vzl.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://lat.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vys.yangfankeji.com

JS:   console.error("err")
来源：http://hhs.mhx1999.top

TS:   console.error("err")
来源：http://qvr.svipenyu.cn

Java: System.err.println("err")
来源：http://odz.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ash.yonumen.top

Ruby: warn "err"
来源：http://qes.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://hbn.fktsv.cn

[M07] 判断是否为主入口
来源：http://rid.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://rxp.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tsz.vqdsnc.cn

JS:   require.main === module
来源：http://jbl.chenzaomai.com

TS:   require.main === module
来源：http://tti.bbcook.cn

Java: public static void main(String[] args)
来源：http://zcx.shuidangran.top

Go:   func main()
来源：http://ymk.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zbr.xylfe.cn

C#:   static void Main(string[] args)
来源：http://asl.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://kkc.yfazqb.com

Py:   platform.system();  platform.python_version()
来源：http://dcn.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://wbk.birdmap.top

JS:   process.platform;  process.version
来源：http://njr.zhengqikj.top

TS:   process.platform;  process.version
来源：http://ssh.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xzq.fengsongda.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://voy.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eyb.redwolf501.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zcz.zhixingplan.top

================================================================================
来源：http://nzf.haohaochexian.top

N. 数据结构与算法
来源：http://bjg.52xcode.cn

================================================================================
来源：http://xfb.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://ehg.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gav.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://slk.zhoulong.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qrh.hnxiangtu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tsh.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://cus.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://fjp.zhijiandao.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qii.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://ymw.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://pfl.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://nep.yj20258.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bdv.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yep.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://cwz.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wue.wangdashe.top

Go:   slices.Sort(arr)
来源：http://xvk.meibo888.top

Ruby: arr.sort
来源：http://nak.ivvv.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://edq.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://xqi.andypj.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jyt.iojbl.cn

PHP:  // 递归实现，或用 usort
来源：http://uqd.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ddj.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://owo.yongpay.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kbd.hfpthk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ptk.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yrx.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jeu.zycfv.cn

[N04] 斐波那契数列
来源：http://mju.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rkl.hongshengwenyu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kxp.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ngi.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jnj.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uoz.nanxuanxn.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zpk.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rja.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zjv.ivvv.top

[N05] 最大公约数
来源：http://epq.fzhhl.top

Py:   math.gcd(a, b)
来源：http://qpk.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tnr.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fiq.c1oappe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hqh.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://onf.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fwf.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://xpr.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lhv.quarkkingdee.top

[N06] 判断回文字符串
来源：http://pnl.hongshengwenyu.top

Py:   s == s[::-1]
来源：http://miz.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://hfq.tarul.cn

JS:   s === [...s].reverse().join("")
来源：http://qhr.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://wnx.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://awg.vqdsnc.cn

Go:   // 双指针从两端比较
来源：http://pqm.chenzaomai.com

Ruby: s == s.reverse
来源：http://rfp.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ugm.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://avn.0kj1m.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://shc.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://esz.xylfe.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rlp.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://qsx.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://gvz.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://wfj.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://gef.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://pww.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://zfg.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://yxb.hammf.cn

PHP:  // 手写递归交换
来源：http://lqz.bjfxy.top

JS:   // 手写回溯递归
来源：http://jwt.havefunace.top

TS:   // 手写回溯递归
来源：http://cci.cdnleiting.top

Java: // 手写回溯递归
来源：http://fnc.ywan-chungtsiang.top

Go:   // 手写回溯递归
来源：http://wki.zhoulong.xyz

Ruby: arr.permutation.to_a
来源：http://nyv.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://hiy.dashuyun.cn

[N09] 栈与队列
来源：http://hdg.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lnp.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ffr.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hhq.yueranfly.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rfy.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qaa.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jyz.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iav.tian-w.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cci.hesvh.cn

[N10] 链表节点定义
来源：http://cjm.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://olb.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lbq.yongpay.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qkr.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gor.yj202588.top

Java: class Node { int v; Node next; }
来源：http://ekb.guowangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://tkz.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xsx.sufxvd.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bxd.pycfn.com

[N11] 二叉树中序遍历
来源：http://pkl.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lte.yj202588.top

PHP:  // 手写递归函数
来源：http://aqs.snrcjt.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blc.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mrg.cucudq.cn

Java: // 手写递归
来源：http://iss.sweek.top

Go:   // 手写递归
来源：http://shn.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://woy.nanxinkj.top

C#:   // 手写递归
来源：http://nah.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fas.yangfankeji.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gjg.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bdb.ppjwa.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xhv.aizwys.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gqs.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tga.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fjx.gogol.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vgd.chenzaomai.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lqa.fzhhl.top

================================================================================
来源：http://usb.fengsongda.top

O. 并发与异步
来源：http://xqu.yuxming.cn

================================================================================
来源：http://zsf.yvedp.cn

[O01] 启动一个线程
来源：http://tpn.yj20258888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jsa.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://npq.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rae.zdqjudy.top

TS:   // 同 JS
来源：http://odz.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://srl.52xcode.cn

Go:   go f()
来源：http://oko.zhiwuduotai.top

Ruby: Thread.new { f }
来源：http://ota.hammf.cn

C#:   Task.Run(() => F());
来源：http://jqb.shangyingyoupin.top

[O02] 使用线程池
来源：http://hqn.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sne.fengsongda.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vhc.jlsjyb.cn

JS:   // worker_threads 线程池
来源：http://iyu.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://nyj.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://bke.jqgfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aos.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ltr.cdnleiting.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uzk.cheryme.top

[O03] 加锁保护共享数据
来源：http://mni.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://urp.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://fqk.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oyp.gogol.net.cn

TS:   // 同 JS
来源：http://wdz.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://nyn.vqdsnc.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mvh.daria6918.cn


<!-- 参考信息 -->