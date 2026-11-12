代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ype.52xcode.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tgu.hysaishi.cn

[K08] 二进制序列化（非 JSON）
来源：http://kad.cucudq.cn

Py:   pickle.dumps(obj)
来源：http://ptp.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nyr.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://fji.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://jdz.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gdm.yj20258888.top

Go:   encoding/gob
来源：http://uxg.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://wil.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sap.zhoulong.xyz

================================================================================
来源：http://hhb.svipenyu.cn

L. 网络请求
来源：http://iro.yangfankeji.com

================================================================================
来源：http://aiw.smart0.xyz

[L01] 发送 GET 请求
来源：http://ypc.yj20258888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ayd.xuanzx.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xjb.chenlongwang.top

JS:   await fetch(url)
来源：http://ewc.cheryme.top

TS:   await fetch(url)
来源：http://lmp.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pxf.52xcode.cn

Go:   resp, err := http.Get(url)
来源：http://ugq.guowangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cfk.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xah.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://kjh.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ics.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ebw.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qak.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nmg.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://avp.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hsr.yanxiufei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yts.yonumen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://juh.havefunace.top

[L03] 设置自定义请求头
来源：http://zvq.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vpq.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://txs.xinyue.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jhu.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bwe.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tqz.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hff.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ykm.bbcook.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://axj.ppjwa.cn

[L04] 设置超时
来源：http://mhs.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://xah.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dce.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ghy.yanxiufei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lmw.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://opc.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uvl.hywenlv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xwj.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mwn.ydzc1.top

[L05] 上传文件（multipart）
来源：http://dwk.nanxuanxn.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ugp.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tkx.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fki.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pqu.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://stc.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xjt.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cue.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rgi.zdbjq.cn

[L06] 解析响应为 JSON
来源：http://vei.yongpay.top

Py:   resp.json()
来源：http://nmb.gotoacloud.top

PHP:  json_decode($body, true);
来源：http://ljh.sjlbkw.cn

JS:   await resp.json()
来源：http://lzy.hcnkem.com

TS:   await resp.json()
来源：http://drl.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zlh.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://atg.bbcook.cn

Ruby: JSON.parse(resp.body)
来源：http://rbg.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://szj.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://sgi.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gbk.mhx1999.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yhx.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://tyo.fktsv.cn

TS:   resp.ok;  resp.status
来源：http://gpt.haohaochexian.top

Java: resp.statusCode()
来源：http://oqr.aizwys.cn

Go:   resp.StatusCode
来源：http://aii.tanke756.top

Ruby: resp.code.to_i
来源：http://jyy.cqqwz.cn

C#:   (int)resp.StatusCode
来源：http://tpp.nwbrower.top

[L08] 并发请求多个地址
来源：http://zjc.hcnkem.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nlr.shuidangran.top

PHP:  curl_multi_init() 系列
来源：http://hqa.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ayo.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ivs.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pdh.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dvk.xylfe.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nrn.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qgz.cheryme.top

================================================================================
来源：http://poc.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://zzz.yuxming.cn

================================================================================
来源：http://lxv.gotoacloud.top

[M01] 读取命令行参数
来源：http://iki.birdmap.top

Py:   sys.argv[1:]
来源：http://tnv.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://zwq.fehbvm.com

JS:   process.argv.slice(2)
来源：http://fra.cheryme.top

TS:   process.argv.slice(2)
来源：http://oid.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://uvf.xuetiantiany.cn

Go:   os.Args[1:]
来源：http://pfp.jinyuanbaomall.cn

Ruby: ARGV
来源：http://gfb.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://vze.9152youxi.cn

[M02] 读取环境变量
来源：http://hoj.316326.xyz

Py:   os.environ.get("HOME")
来源：http://mhx.hfpthk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yex.zhixingplan.top

JS:   process.env.HOME
来源：http://wwd.gzhubu.top

TS:   process.env.HOME
来源：http://tpv.sufxvd.cn

Java: System.getenv("HOME")
来源：http://kqb.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vat.xinyue.icu

Ruby: ENV["HOME"]
来源：http://aug.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://abc.quarkkingdee.top

[M03] 执行外部命令
来源：http://gky.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://txa.chenzaomai.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zlz.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://sbq.ydzc1.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kco.chenjidiqi.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cer.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gko.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://cee.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://uzn.xinyue.icu

[M04] 获取当前工作目录
来源：http://bto.yfazqb.com

Py:   os.getcwd()
来源：http://qfe.shzxlz.cn

PHP:  getcwd();
来源：http://uqg.gzhubu.top

JS:   process.cwd()
来源：http://ufm.nanxuanxn.top

TS:   process.cwd()
来源：http://vqs.sweek.top

Java: Path.of("").toAbsolutePath()
来源：http://tek.ctjpmb.com

Go:   os.Getwd()
来源：http://qik.nwbrower.top

Ruby: Dir.pwd
来源：http://icr.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://lah.jqgfzy.top

[M05] 设置退出码
来源：http://hay.cashguo.top

Py:   sys.exit(1)
来源：http://heq.gogol.net.cn

PHP:  exit(1);
来源：http://xyt.ydjk.org.cn

JS:   process.exit(1)
来源：http://pqa.cdnleiting.top

TS:   process.exit(1)
来源：http://gxi.316326.xyz

Java: System.exit(1)
来源：http://cul.nanxuanxn.top

Go:   os.Exit(1)
来源：http://xct.zhengqikj.top

Ruby: exit 1
来源：http://rjb.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://usk.daria6918.cn

[M06] 向标准错误输出
来源：http://xal.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://fcf.xinyue.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://fkz.yuxming.cn

JS:   console.error("err")
来源：http://zba.zhaomingkeji.xyz

TS:   console.error("err")
来源：http://vxl.hcnkem.com

Java: System.err.println("err")
来源：http://xog.quarkkingdee.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://osk.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://qzn.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://iez.jqgfzy.top

[M07] 判断是否为主入口
来源：http://dwn.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://nbw.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mih.bjfxy.top

JS:   require.main === module
来源：http://qei.jyoumei.cn

TS:   require.main === module
来源：http://xnn.xziqi.cn

Java: public static void main(String[] args)
来源：http://uyy.fzhhl.top

Go:   func main()
来源：http://bog.tian-w.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://its.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://ahe.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://xhf.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://ega.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://ebv.yfazqb.com

JS:   process.platform;  process.version
来源：http://mgi.fehbvm.com

TS:   process.platform;  process.version
来源：http://tyh.zdqjudy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ump.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://npy.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gqe.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://epy.jinqigufen.top

================================================================================
来源：http://qwr.nwbrower.top

N. 数据结构与算法
来源：http://fqs.sweek.top

================================================================================
来源：http://uvd.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://ugo.zdqjudy.top

Py:   bisect.bisect_left(arr, x)
来源：http://evv.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://naf.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://glb.snrcjt.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ufd.wangshuangyany.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tsa.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://iyf.nwbrower.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://saa.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://cnn.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://ucj.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://gnu.hnxiangtu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ssi.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lkq.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dac.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dlg.xuanzx.com

Go:   slices.Sort(arr)
来源：http://vcc.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://kej.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://coy.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://edr.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jaq.fehbvm.com

PHP:  // 递归实现，或用 usort
来源：http://uyo.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gxb.wangdashe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hqy.epnwcf.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xqc.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zcd.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dgl.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://gqp.yuxming.cn

[N04] 斐波那契数列
来源：http://ces.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nrb.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nri.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mhz.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cqs.xylfe.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eqj.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jcs.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sqv.xuanzx.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kdm.yfazqb.com

[N05] 最大公约数
来源：http://tdh.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://vro.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mou.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://img.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ibo.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qxh.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pdo.chenzaomai.com

Ruby: a.gcd(b)
来源：http://gwq.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fsz.smart0.xyz

[N06] 判断回文字符串
来源：http://xqa.gaohongyu789.top

Py:   s == s[::-1]
来源：http://yfk.gogol.net.cn

PHP:  $s === strrev($s);
来源：http://gma.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://wot.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://lcq.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pni.feifeiyinyue.top

Go:   // 双指针从两端比较
来源：http://gkt.guowangkeji.top

Ruby: s == s.reverse
来源：http://uvo.9152youxi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fen.cheryme.top

[N07] 两数之和（返回下标）
来源：http://umi.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lhk.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mic.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://lgj.0kj1m.cn

TS:   // 手写 Map<string, number>
来源：http://upo.yueranfly.top

Java: // 手写 HashMap
来源：http://urk.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://aei.daria6918.cn

Ruby: // 手写 Hash
来源：http://wup.vehdjk.com

C#:   // 手写 Dictionary<int, int>
来源：http://tad.cheryme.top

[N08] 生成全排列
来源：http://dqi.snrcjt.cn

Py:   itertools.permutations(arr)
来源：http://xhw.quarkkingdee.top

PHP:  // 手写递归交换
来源：http://ebr.zdqjudy.top

JS:   // 手写回溯递归
来源：http://imz.yj202588.top

TS:   // 手写回溯递归
来源：http://lkk.yonumen.top

Java: // 手写回溯递归
来源：http://czh.fengsongda.top

Go:   // 手写回溯递归
来源：http://qvt.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://fsc.yj20258.top

C#:   // 手写回溯递归
来源：http://kre.zhengqikj.top

[N09] 栈与队列
来源：http://yvd.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ept.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ipf.cheryme.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rfs.shangyingyoupin.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://crt.yongpay.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zwt.sysykeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ddx.jiagoushi.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qjc.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://utl.316326.xyz

[N10] 链表节点定义
来源：http://emc.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zxd.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qvl.hcnkem.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mer.jinqigfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cws.yuxming.cn

Java: class Node { int v; Node next; }
来源：http://kpa.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://rva.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ans.mhx1999.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jtv.jqgufenzy.top

[N11] 二叉树中序遍历
来源：http://dxx.jinqigfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sjy.ctjpmb.com

PHP:  // 手写递归函数
来源：http://txh.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zfa.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kro.zhijiandao.cn

Java: // 手写递归
来源：http://gks.yanxiufei.cn

Go:   // 手写递归
来源：http://hqq.cdnleiting.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ren.316326.xyz

C#:   // 手写递归
来源：http://jtv.gogol.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nxw.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sxs.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oxs.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kko.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xhc.ehwqpu.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iwq.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vlo.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xez.ctjpmb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bqn.shanyushiyangkeji.top

================================================================================
来源：http://weo.ctjpmb.com

O. 并发与异步
来源：http://zea.sufxvd.cn

================================================================================
来源：http://gxo.bjfxy.top

[O01] 启动一个线程
来源：http://las.birdmap.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hkg.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ajh.shuidangran.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xhg.zhongyouzk.top

TS:   // 同 JS
来源：http://lzs.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://xnr.shangyingyoupin.top

Go:   go f()
来源：http://xfh.hcnkem.com

Ruby: Thread.new { f }
来源：http://fdn.zhoulong.xyz

C#:   Task.Run(() => F());
来源：http://fwy.xylfe.cn

[O02] 使用线程池
来源：http://hri.quarkkingdee.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kjs.wangshuangyany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sbl.hcnkem.com

JS:   // worker_threads 线程池
来源：http://nzj.hfpthk.cn

TS:   // worker_threads 线程池
来源：http://hnc.pengpengdd.cyou

Java: Executors.newFixedThreadPool(4)
来源：http://ara.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rxx.gotoacloud.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bco.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zix.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://dta.zdbjq.cn

Py:   with lock: shared += 1
来源：http://vsl.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://wdg.jlsjyb.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cro.gotoacloud.top

TS:   // 同 JS
来源：http://jgv.shanyushiyangtech.top

Java: synchronized (this) { shared++; }
来源：http://ods.havefunace.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hmb.0kj1m.cn


<!-- 参考信息 -->