代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zah.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dxn.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zgl.shanyushiyangtech.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wmt.fengsongda.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gjh.shangyingyoupin.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cij.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://hls.sxryk.cn

Py:   pickle.dumps(obj)
来源：http://lil.aibaodan.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nmr.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://pwc.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://kno.fehbvm.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mec.gaohongyu789.top

Go:   encoding/gob
来源：http://wtk.vqdsnc.cn

Ruby: Marshal.dump(obj)
来源：http://uja.hysaishi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://axv.c1oappe.top

================================================================================
来源：http://yvp.quarkkingdee.top

L. 网络请求
来源：http://ava.havefunace.top

================================================================================
来源：http://dme.zhengqikj.top

[L01] 发送 GET 请求
来源：http://gjj.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wys.cashguo.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qjb.cqqwz.cn

JS:   await fetch(url)
来源：http://gxu.hywenlv.cn

TS:   await fetch(url)
来源：http://utg.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nvj.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://fal.zycfv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fth.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://exo.xziqi.cn

[L02] 发送 POST JSON
来源：http://qyy.nwbrower.top

Py:   requests.post(url, json={"a": 1})
来源：http://gki.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mkc.hnxiangtu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wzl.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://osy.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uyh.fktsv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xbu.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vws.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gtz.xingfuxueyuan.xyz

[L03] 设置自定义请求头
来源：http://zpa.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://khj.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oig.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uws.zhoulong.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gmr.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ycj.yonumen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bso.mhx1999.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://npa.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ujp.hongshengwenyu.top

[L04] 设置超时
来源：http://hoo.zdqjudy.top

Py:   requests.get(url, timeout=5)
来源：http://ffv.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fed.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xgf.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qsr.hysaishi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://awe.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://osp.hnxiangtu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://urv.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yeh.ctjpmb.com

[L05] 上传文件（multipart）
来源：http://osp.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lht.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fiz.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://utl.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ujc.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://azf.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dyw.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vwq.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://det.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://gic.birdmap.top

Py:   resp.json()
来源：http://ioq.tarul.cn

PHP:  json_decode($body, true);
来源：http://keh.yueranfly.top

JS:   await resp.json()
来源：http://zea.gogol.net.cn

TS:   await resp.json()
来源：http://ckz.gotoacloud.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cqm.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rit.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://hav.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fas.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://bwl.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xah.nanxinkj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://phv.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://gyy.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://gxg.daria6918.cn

Java: resp.statusCode()
来源：http://wxd.cheryme.top

Go:   resp.StatusCode
来源：http://pvj.epnwcf.com

Ruby: resp.code.to_i
来源：http://pyq.yueranfly.top

C#:   (int)resp.StatusCode
来源：http://ptf.ctjpmb.com

[L08] 并发请求多个地址
来源：http://hwi.zhiwuduotai.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oqf.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://qlk.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xrr.jianghu66.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://num.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iuw.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bsj.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dqg.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://myh.yuanzhike.top

================================================================================
来源：http://jsw.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://dfq.hfpthk.cn

================================================================================
来源：http://gjl.jqgufenzy.top

[M01] 读取命令行参数
来源：http://jny.cdnleiting.top

Py:   sys.argv[1:]
来源：http://myt.tarul.cn

PHP:  $argv;  $argc;
来源：http://vlw.jianghu66.top

JS:   process.argv.slice(2)
来源：http://dvu.aizwys.cn

TS:   process.argv.slice(2)
来源：http://bxc.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://bxh.zhixingplan.top

Go:   os.Args[1:]
来源：http://xso.yj202588.top

Ruby: ARGV
来源：http://ykw.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://rxf.hnxiangtu.top

[M02] 读取环境变量
来源：http://fyp.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://sft.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://geo.nanxinkj.top

JS:   process.env.HOME
来源：http://nbi.xuetiantiany.cn

TS:   process.env.HOME
来源：http://gtu.smart0.xyz

Java: System.getenv("HOME")
来源：http://ost.c1oappe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://flj.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://zjr.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://esd.xylfe.cn

[M03] 执行外部命令
来源：http://qvm.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mvr.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gzw.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fdf.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pjt.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fpd.guowangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mdt.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xeg.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://nhr.yj20258888.top

[M04] 获取当前工作目录
来源：http://dsu.guannengcc.top

Py:   os.getcwd()
来源：http://ukj.chenlongwang.top

PHP:  getcwd();
来源：http://ant.sxryk.cn

JS:   process.cwd()
来源：http://okz.sweek.top

TS:   process.cwd()
来源：http://lsh.zhijiandao.cn

Java: Path.of("").toAbsolutePath()
来源：http://xya.nanxuanxn.top

Go:   os.Getwd()
来源：http://flo.zhoulong.xyz

Ruby: Dir.pwd
来源：http://sqn.xylfe.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dut.jiagoushi.top

[M05] 设置退出码
来源：http://wsw.yangfankeji.com

Py:   sys.exit(1)
来源：http://qrk.redwolf501.top

PHP:  exit(1);
来源：http://hbt.cdnleiting.top

JS:   process.exit(1)
来源：http://vmy.jqgfzy.top

TS:   process.exit(1)
来源：http://hct.jinghuilouyu.cn

Java: System.exit(1)
来源：http://yna.fktsv.cn

Go:   os.Exit(1)
来源：http://kcb.yj202588.top

Ruby: exit 1
来源：http://ora.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ytk.xylfe.cn

[M06] 向标准错误输出
来源：http://qqi.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://tmd.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yjr.haohaochexian.top

JS:   console.error("err")
来源：http://nyl.yuxming.cn

TS:   console.error("err")
来源：http://vgq.yj20258888.top

Java: System.err.println("err")
来源：http://add.guannengcc.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ccc.smart0.xyz

Ruby: warn "err"
来源：http://utr.ydzc1.top

C#:   Console.Error.WriteLine("err")
来源：http://kfz.meibo888.top

[M07] 判断是否为主入口
来源：http://jaq.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://ovt.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wve.xuanzx.com

JS:   require.main === module
来源：http://eda.zhongyouzk.top

TS:   require.main === module
来源：http://cqz.yuxming.cn

Java: public static void main(String[] args)
来源：http://nhh.zhongyouzk.top

Go:   func main()
来源：http://dmp.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xov.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://scy.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://aii.meibo888.top

Py:   platform.system();  platform.python_version()
来源：http://ibv.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://azr.yonumen.top

JS:   process.platform;  process.version
来源：http://btl.gzhubu.top

TS:   process.platform;  process.version
来源：http://hqu.sjlbkw.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pzg.xuanzx.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://hsc.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hrg.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rhm.daxiang520.top

================================================================================
来源：http://jyp.chenjidiqi.icu

N. 数据结构与算法
来源：http://joz.shzxlz.cn

================================================================================
来源：http://lnw.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://qih.vqdsnc.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wkx.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bvz.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gag.kuanghao11.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lte.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://kfd.52xcode.cn

Go:   sort.SearchInts(arr, x)
来源：http://ksp.yangfankeji.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ocr.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://mfu.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://uri.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://pja.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gne.yanxiufei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yrk.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://wlc.vqdsnc.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pft.ivvv.top

Go:   slices.Sort(arr)
来源：http://bvm.ivvv.top

Ruby: arr.sort
来源：http://ilw.feifeiyinyue.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://iat.yvedp.cn

[N03] 快速排序（分治示例）
来源：http://ckb.ydjk.org.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kvp.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://dto.9152youxi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bgs.yfazqb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nkb.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://efy.andypj.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://arf.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kqy.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://vtk.wangdashe.top

[N04] 斐波那契数列
来源：http://qme.xziqi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vjz.jqgfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uvj.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ecv.jiagoushi.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jih.tianlin.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cft.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mzm.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kfu.yanxiufei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jrj.yangfankeji.com

[N05] 最大公约数
来源：http://ixh.meibo888.top

Py:   math.gcd(a, b)
来源：http://vfh.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://feg.dashuyun.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xgv.svipenyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wvb.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bjv.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lbf.gogol.net.cn

Ruby: a.gcd(b)
来源：http://cri.cheryme.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vpr.c1oappe.top

[N06] 判断回文字符串
来源：http://wba.hfpthk.cn

Py:   s == s[::-1]
来源：http://ufw.52xcode.cn

PHP:  $s === strrev($s);
来源：http://rbm.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://hso.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://azk.zycfv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pyk.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://kpq.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://nzc.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tnn.chenlongwang.top

[N07] 两数之和（返回下标）
来源：http://wiq.hnqzz.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ohf.zdqjudy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dkh.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://lux.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://wae.fengsongda.top

Java: // 手写 HashMap
来源：http://gxt.yonumen.top

Go:   // 手写 map[int]int
来源：http://cfo.sxryk.cn

Ruby: // 手写 Hash
来源：http://dyj.tanke756.top

C#:   // 手写 Dictionary<int, int>
来源：http://ymu.sufxvd.cn

[N08] 生成全排列
来源：http://nut.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://arn.epnwcf.com

PHP:  // 手写递归交换
来源：http://uzo.tianlin.xyz

JS:   // 手写回溯递归
来源：http://acl.hesvh.cn

TS:   // 手写回溯递归
来源：http://yuw.xziqi.cn

Java: // 手写回溯递归
来源：http://qkn.pengpengdd.cyou

Go:   // 手写回溯递归
来源：http://dva.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://vjz.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://xvp.jlsjyb.cn

[N09] 栈与队列
来源：http://gex.hammf.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lqx.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cyk.hammf.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ubs.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qov.cashguo.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tzn.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bbc.jianghu66.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qgq.yj20258888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yfp.sysykeji.top

[N10] 链表节点定义
来源：http://oel.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xuo.havefunace.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dhn.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lwh.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lvx.cucudq.cn

Java: class Node { int v; Node next; }
来源：http://hhf.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://rlz.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://ija.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jem.yangfankeji.com

[N11] 二叉树中序遍历
来源：http://xbz.shanyushiyangtech.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vft.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://cki.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pqf.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://byv.iojbl.cn

Java: // 手写递归
来源：http://dxg.fanxiaobao.xyz

Go:   // 手写递归
来源：http://mzb.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qti.mhx1999.top

C#:   // 手写递归
来源：http://dtk.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kks.jinqigufen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://stj.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mph.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dea.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xch.chenjidiqi.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bhf.hysaishi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pfx.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iml.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zua.shangyingyoupin.top

================================================================================
来源：http://pyi.daria6918.cn

O. 并发与异步
来源：http://yic.yj20258888.top

================================================================================
来源：http://baq.gaohongyu789.top

[O01] 启动一个线程
来源：http://wgs.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kus.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qpz.vqdsnc.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nrj.zycfv.cn

TS:   // 同 JS
来源：http://hdy.zhijiandao.cn

Java: new Thread(() -> f()).start()
来源：http://dms.yj20258.top

Go:   go f()
来源：http://wnj.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://kfb.sufxvd.cn

C#:   Task.Run(() => F());
来源：http://duf.aibaodan.cn

[O02] 使用线程池
来源：http://hnj.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://juw.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lkh.chenjidiqi.icu

JS:   // worker_threads 线程池
来源：http://hiq.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://wff.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://gps.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://efm.hcnkem.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lle.hnxiangtu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://upm.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://vhw.havefunace.top

Py:   with lock: shared += 1
来源：http://swy.vqdsnc.cn

PHP:  // 用 flock() 做文件锁
来源：http://kvl.shanyushiyangkeji.top


<!-- 参考信息 -->