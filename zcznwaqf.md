代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dzy.ywan-chungtsiang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lek.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qui.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fty.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://efz.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uas.hysaishi.cn

[K08] 二进制序列化（非 JSON）
来源：http://peo.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://gdm.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gea.xziqi.cn

JS:   v8.serialize(obj)        // Node
来源：http://pph.pengpengdd.cyou

TS:   v8.serialize(obj)        // Node
来源：http://rsb.fehbvm.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://isi.ywan-chungtsiang.top

Go:   encoding/gob
来源：http://vir.yj202588.top

Ruby: Marshal.dump(obj)
来源：http://eix.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eqt.shzxlz.cn

================================================================================
来源：http://fhp.hnxiangtu.top

L. 网络请求
来源：http://ghb.ydzc1.top

================================================================================
来源：http://dor.xingfuxueyuan.xyz

[L01] 发送 GET 请求
来源：http://jel.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hil.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://unr.jianghu66.top

JS:   await fetch(url)
来源：http://ygi.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://pad.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cbj.yongpay.top

Go:   resp, err := http.Get(url)
来源：http://jll.sufxvd.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://oou.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kto.dashuyun.cn

[L02] 发送 POST JSON
来源：http://pmg.jinqigufen.top

Py:   requests.post(url, json={"a": 1})
来源：http://nwc.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lde.chenzaomai.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kla.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lzt.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rva.hammf.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fvf.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fip.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rkp.ywan-chungtsiang.top

[L03] 设置自定义请求头
来源：http://vfg.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://srb.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zbr.tian-w.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nbg.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vbx.nanxinkj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://htl.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hgi.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://opx.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nsb.iojbl.cn

[L04] 设置超时
来源：http://txk.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://bvm.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tek.hesvh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vzo.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zxx.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oxs.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jyq.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rch.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gkv.mhx1999.top

[L05] 上传文件（multipart）
来源：http://tzj.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yud.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rnt.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wmq.shuidangran.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lde.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rag.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yev.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://alz.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qhr.yanxiufei.cn

[L06] 解析响应为 JSON
来源：http://ojs.pengpengdd.cyou

Py:   resp.json()
来源：http://cec.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://pba.ivvv.top

JS:   await resp.json()
来源：http://fkn.xziqi.cn

TS:   await resp.json()
来源：http://qoy.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://awu.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://flw.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://exa.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xvr.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://wwu.chenjidiqi.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fzi.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pzw.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://fgy.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://elh.yj20258.top

Java: resp.statusCode()
来源：http://kfe.redwolf501.top

Go:   resp.StatusCode
来源：http://fqe.hfpthk.cn

Ruby: resp.code.to_i
来源：http://jvv.c1oappe.top

C#:   (int)resp.StatusCode
来源：http://fir.hysaishi.cn

[L08] 并发请求多个地址
来源：http://zxb.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ius.daxiang520.top

PHP:  curl_multi_init() 系列
来源：http://tsi.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hpr.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qgi.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pmp.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xkq.cashguo.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://for.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ijr.hfpthk.cn

================================================================================
来源：http://dbm.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://bfj.aizwys.cn

================================================================================
来源：http://trq.yonumen.top

[M01] 读取命令行参数
来源：http://hdr.jiagoushi.top

Py:   sys.argv[1:]
来源：http://uus.tarul.cn

PHP:  $argv;  $argc;
来源：http://gfr.yongpay.top

JS:   process.argv.slice(2)
来源：http://waa.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://led.0kj1m.cn

Java: args 数组（main 方法参数）
来源：http://fpd.52xcode.cn

Go:   os.Args[1:]
来源：http://ypm.sweek.top

Ruby: ARGV
来源：http://pkk.xylfe.cn

C#:   args 数组（Main 方法参数）
来源：http://hfs.uphjek.com

[M02] 读取环境变量
来源：http://lbk.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://jjb.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qbr.aizwys.cn

JS:   process.env.HOME
来源：http://mmz.xinyue.icu

TS:   process.env.HOME
来源：http://dag.hysaishi.cn

Java: System.getenv("HOME")
来源：http://gtx.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zwx.xziqi.cn

Ruby: ENV["HOME"]
来源：http://oae.xinyue.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tmo.vqdsnc.cn

[M03] 执行外部命令
来源：http://tbv.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ozi.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ixp.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pes.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fzn.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bay.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zja.yj20258888.top

Ruby: system("ls -l");  `ls -l`
来源：http://hlp.zhijiandao.cn

C#:   Process.Start("ls", "-l");
来源：http://ugv.zhixingplan.top

[M04] 获取当前工作目录
来源：http://erh.chenzaomai.com

Py:   os.getcwd()
来源：http://qbg.dianchejie.cn

PHP:  getcwd();
来源：http://vjh.zhixingplan.top

JS:   process.cwd()
来源：http://ykh.vqdsnc.cn

TS:   process.cwd()
来源：http://ems.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://ppi.yongpay.top

Go:   os.Getwd()
来源：http://tmv.snrcjt.cn

Ruby: Dir.pwd
来源：http://gde.jinqigfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://hbr.bbcook.cn

[M05] 设置退出码
来源：http://uju.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://qau.hywenlv.cn

PHP:  exit(1);
来源：http://iix.zhijiandao.cn

JS:   process.exit(1)
来源：http://qfx.xylfe.cn

TS:   process.exit(1)
来源：http://msi.feifeiyinyue.top

Java: System.exit(1)
来源：http://ewu.jyoumei.cn

Go:   os.Exit(1)
来源：http://vsd.pycfn.com

Ruby: exit 1
来源：http://qxc.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nfk.fehbvm.com

[M06] 向标准错误输出
来源：http://ndi.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://myb.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jai.fzhhl.top

JS:   console.error("err")
来源：http://spc.sysykeji.top

TS:   console.error("err")
来源：http://jbo.yj20258.top

Java: System.err.println("err")
来源：http://uph.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://asd.nwbrower.top

Ruby: warn "err"
来源：http://nwi.shangyingyoupin.top

C#:   Console.Error.WriteLine("err")
来源：http://sfg.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://phd.smart0.xyz

Py:   if __name__ == "__main__":
来源：http://ues.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nnu.pengpengdd.cyou

JS:   require.main === module
来源：http://qzl.yangfankeji.com

TS:   require.main === module
来源：http://ncv.pycfn.com

Java: public static void main(String[] args)
来源：http://lyw.zhengqikj.top

Go:   func main()
来源：http://spd.andypj.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://igu.daria6918.cn

C#:   static void Main(string[] args)
来源：http://taf.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://nzv.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://hxy.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://erl.gzhubu.top

JS:   process.platform;  process.version
来源：http://osw.hongshengwenyu.top

TS:   process.platform;  process.version
来源：http://lln.quarkkingdee.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qre.yj20258.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hak.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://twg.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vwg.jiagoushi.top

================================================================================
来源：http://dry.c1oappe.top

N. 数据结构与算法
来源：http://zlb.havefunace.top

================================================================================
来源：http://zpo.sweek.top

[N01] 二分查找（有序数组）
来源：http://ejr.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://brm.hnqzz.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rrh.shanyushiyangtech.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tyi.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mak.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://eag.hongshengwenyu.top

Go:   sort.SearchInts(arr, x)
来源：http://ytl.cqqwz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rud.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://izg.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://ubp.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qvi.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hxc.sweek.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vic.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://paf.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sbp.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://squ.tarul.cn

Ruby: arr.sort
来源：http://odf.smart0.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://aaw.meibo888.top

[N03] 快速排序（分治示例）
来源：http://xso.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://niq.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://ocp.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://umd.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kcj.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://irh.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uqk.jyoumei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ytt.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://spc.cheryme.top

[N04] 斐波那契数列
来源：http://tqj.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nnm.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://buh.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yfu.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://foy.dianchejie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mrf.birdmap.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nwh.zhijiandao.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zhe.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gli.gogol.net.cn

[N05] 最大公约数
来源：http://wgk.ivvv.top

Py:   math.gcd(a, b)
来源：http://coe.andypj.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kwb.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wjm.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hqi.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bpf.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ztr.fehbvm.com

Ruby: a.gcd(b)
来源：http://awv.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aev.mhx1999.top

[N06] 判断回文字符串
来源：http://djr.yonumen.top

Py:   s == s[::-1]
来源：http://gmu.tian-w.cn

PHP:  $s === strrev($s);
来源：http://lrw.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://zpg.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://kxm.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zsb.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://ohd.c1oappe.top

Ruby: s == s.reverse
来源：http://ksd.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nkn.yongpay.top

[N07] 两数之和（返回下标）
来源：http://sgr.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lrj.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fti.yongpay.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gfb.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://mli.yvedp.cn

Java: // 手写 HashMap
来源：http://yky.xuetiantiany.cn

Go:   // 手写 map[int]int
来源：http://yib.gogol.net.cn

Ruby: // 手写 Hash
来源：http://wwh.uphjek.com

C#:   // 手写 Dictionary<int, int>
来源：http://nho.tianlin.xyz

[N08] 生成全排列
来源：http://wty.shzxlz.cn

Py:   itertools.permutations(arr)
来源：http://crt.ivvv.top

PHP:  // 手写递归交换
来源：http://sqb.ctjpmb.com

JS:   // 手写回溯递归
来源：http://lya.havefunace.top

TS:   // 手写回溯递归
来源：http://rkw.jinqigufen.top

Java: // 手写回溯递归
来源：http://jmz.zdqjudy.top

Go:   // 手写回溯递归
来源：http://aup.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://orp.zdqjudy.top

C#:   // 手写回溯递归
来源：http://xws.chenzaomai.com

[N09] 栈与队列
来源：http://jdy.wangshuangyany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pzy.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vdl.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jqz.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zpl.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oww.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://opv.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nsf.xylfe.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lgb.yonumen.top

[N10] 链表节点定义
来源：http://pus.zhiwuduotai.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jnk.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mfp.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qcv.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tau.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://psd.yueranfly.top

Go:   type Node struct { V int; Next *Node }
来源：http://cpy.zhijiandao.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bad.sysykeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://oyo.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://rhk.jinghuilouyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sny.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://jnu.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://unj.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://feh.fktsv.cn

Java: // 手写递归
来源：http://lyh.hammf.cn

Go:   // 手写递归
来源：http://efm.aibaodan.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wcf.sxryk.cn

C#:   // 手写递归
来源：http://oob.xinyue.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qel.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yld.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gws.yfazqb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jok.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gjf.shuidangran.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qho.havefunace.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://okd.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qsw.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pkm.zhongyouzk.top

================================================================================
来源：http://yxy.hywenlv.cn

O. 并发与异步
来源：http://lll.andypj.xyz

================================================================================
来源：http://hqn.ivvv.top

[O01] 启动一个线程
来源：http://ipd.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jzd.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qgc.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mlw.jiagoushi.top

TS:   // 同 JS
来源：http://zrf.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://eis.hfpthk.cn

Go:   go f()
来源：http://pna.shzxlz.cn

Ruby: Thread.new { f }
来源：http://pjg.svipenyu.cn

C#:   Task.Run(() => F());
来源：http://yoc.sysykeji.top

[O02] 使用线程池
来源：http://byg.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tnu.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iby.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://oqd.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://yfn.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://zjx.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://epu.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nxo.ppjwa.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yba.vehdjk.com

[O03] 加锁保护共享数据
来源：http://ptb.fanxiaobao.xyz

Py:   with lock: shared += 1
来源：http://muk.0kj1m.cn

PHP:  // 用 flock() 做文件锁
来源：http://exo.52xcode.cn


<!-- 参考信息 -->