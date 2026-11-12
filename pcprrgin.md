代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hcj.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bxc.cucudq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://scj.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ciz.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ahl.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://boe.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://uac.yangfankeji.com

Py:   pickle.dumps(obj)
来源：http://vzh.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uzc.hesvh.cn

JS:   v8.serialize(obj)        // Node
来源：http://pqh.birdmap.top

TS:   v8.serialize(obj)        // Node
来源：http://zqe.xziqi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jiu.havefunace.top

Go:   encoding/gob
来源：http://tzg.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://nov.tian-w.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zvh.aizwys.cn

================================================================================
来源：http://awn.jqgfzy.top

L. 网络请求
来源：http://wou.jqgufenzy.top

================================================================================
来源：http://qlf.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://ckp.jinghuilouyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://txf.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://egr.hcnkem.com

JS:   await fetch(url)
来源：http://pmp.xziqi.cn

TS:   await fetch(url)
来源：http://biq.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lix.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://gmg.kuanghao11.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pze.snrcjt.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bze.ydzc1.top

[L02] 发送 POST JSON
来源：http://qtm.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://myu.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sbz.tian-w.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fel.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xqx.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rnb.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cgu.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pyt.yanxiufei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rwy.zdqjudy.top

[L03] 设置自定义请求头
来源：http://mtx.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cik.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pui.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uiw.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ujs.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ekc.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iez.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hxz.jqgufenzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zxf.zhaomingkeji.xyz

[L04] 设置超时
来源：http://oyp.bjfxy.top

Py:   requests.get(url, timeout=5)
来源：http://apv.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bbo.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xwk.yuxming.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zoc.zhoulong.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wfv.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cyd.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uor.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lst.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://qjd.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ibu.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jyt.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cut.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fma.zycfv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xjf.shanyushiyangtech.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qpw.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nsf.tarul.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yqr.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://qgy.chenjidiqi.icu

Py:   resp.json()
来源：http://hid.tarul.cn

PHP:  json_decode($body, true);
来源：http://oaz.yonumen.top

JS:   await resp.json()
来源：http://iym.yongpay.top

TS:   await resp.json()
来源：http://suw.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ngc.hongshengwenyu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://olr.zhengqikj.top

Ruby: JSON.parse(resp.body)
来源：http://fpt.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bzm.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://tdd.ybcxt.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fgg.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rpf.chenjidiqi.icu

JS:   resp.ok;  resp.status
来源：http://iew.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://nss.tarul.cn

Java: resp.statusCode()
来源：http://wau.ehwqpu.com

Go:   resp.StatusCode
来源：http://pxa.haohaochexian.top

Ruby: resp.code.to_i
来源：http://sve.daria6918.cn

C#:   (int)resp.StatusCode
来源：http://bge.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://nch.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kfp.ywan-chungtsiang.top

PHP:  curl_multi_init() 系列
来源：http://kon.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://api.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://crv.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rnp.yj20258888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ecm.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cdj.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bvq.andypj.xyz

================================================================================
来源：http://tbw.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://elr.hammf.cn

================================================================================
来源：http://iik.yj20258888.top

[M01] 读取命令行参数
来源：http://xob.dianchejie.cn

Py:   sys.argv[1:]
来源：http://rsj.zhaomingkeji.xyz

PHP:  $argv;  $argc;
来源：http://bcc.fktsv.cn

JS:   process.argv.slice(2)
来源：http://ioz.epnwcf.com

TS:   process.argv.slice(2)
来源：http://dgy.yj202588.top

Java: args 数组（main 方法参数）
来源：http://rsp.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://llu.wangshuangyany.cn

Ruby: ARGV
来源：http://zmv.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://jnu.ydzc1.top

[M02] 读取环境变量
来源：http://qdq.gzhubu.top

Py:   os.environ.get("HOME")
来源：http://geg.ywan-chungtsiang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ooh.yuanzhike.top

JS:   process.env.HOME
来源：http://lca.yanxiufei.cn

TS:   process.env.HOME
来源：http://ela.zdqjudy.top

Java: System.getenv("HOME")
来源：http://jvt.havefunace.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jjy.jinghuilouyu.cn

Ruby: ENV["HOME"]
来源：http://rfy.cdnleiting.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ent.gaohongyu789.top

[M03] 执行外部命令
来源：http://aun.zhoulong.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aea.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jbi.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://opt.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gkr.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lbi.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nqj.yj20258.top

Ruby: system("ls -l");  `ls -l`
来源：http://gtz.aibaodan.cn

C#:   Process.Start("ls", "-l");
来源：http://voc.jiagoushi.top

[M04] 获取当前工作目录
来源：http://xlt.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://mcd.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://qzz.yuanzhike.top

JS:   process.cwd()
来源：http://xzq.cashguo.top

TS:   process.cwd()
来源：http://vox.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://inp.gzhubu.top

Go:   os.Getwd()
来源：http://abl.jinqigfzy.top

Ruby: Dir.pwd
来源：http://hql.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zfk.sufxvd.cn

[M05] 设置退出码
来源：http://cxb.aibaodan.cn

Py:   sys.exit(1)
来源：http://upo.yangfankeji.com

PHP:  exit(1);
来源：http://rcf.jqgufenzy.top

JS:   process.exit(1)
来源：http://jkk.andypj.xyz

TS:   process.exit(1)
来源：http://dcd.feifeiyinyue.top

Java: System.exit(1)
来源：http://czx.yj20258.top

Go:   os.Exit(1)
来源：http://snx.xuetiantiany.cn

Ruby: exit 1
来源：http://blk.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xjq.pycfn.com

[M06] 向标准错误输出
来源：http://xoz.cucudq.cn

Py:   print("err", file=sys.stderr)
来源：http://zvv.zhoulong.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://xcl.vehdjk.com

JS:   console.error("err")
来源：http://kbm.havefunace.top

TS:   console.error("err")
来源：http://ftx.hnqzz.top

Java: System.err.println("err")
来源：http://ogn.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tit.guannengcc.top

Ruby: warn "err"
来源：http://eim.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://bpf.cheryme.top

[M07] 判断是否为主入口
来源：http://lvg.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://pse.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mxc.hywenlv.cn

JS:   require.main === module
来源：http://qfu.shzxlz.cn

TS:   require.main === module
来源：http://zvq.uphjek.com

Java: public static void main(String[] args)
来源：http://gwh.shanyushiyangkeji.top

Go:   func main()
来源：http://cye.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qrz.yfazqb.com

C#:   static void Main(string[] args)
来源：http://ldo.guowangkeji.top

[M08] 获取系统与运行时信息
来源：http://fly.daria6918.cn

Py:   platform.system();  platform.python_version()
来源：http://nqq.tianlin.xyz

PHP:  PHP_OS;  phpversion();
来源：http://jgo.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://ast.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://awm.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lbb.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://inf.hammf.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://smy.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ebs.gogol.net.cn

================================================================================
来源：http://cem.ehwqpu.com

N. 数据结构与算法
来源：http://bse.shzxlz.cn

================================================================================
来源：http://iqu.zdqjudy.top

[N01] 二分查找（有序数组）
来源：http://isp.zycfv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ryr.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://svj.chenlongwang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wwl.c1oappe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lhw.jiagoushi.top

Java: Arrays.binarySearch(arr, x)
来源：http://naq.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://itd.jinqigufen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fer.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://rym.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://dqf.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://mhg.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jbi.kuanghao11.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://win.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://nbe.jinghuilouyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nnj.52xcode.cn

Go:   slices.Sort(arr)
来源：http://iqx.zhixingplan.top

Ruby: arr.sort
来源：http://wbc.sjlbkw.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cug.ppjwa.cn

[N03] 快速排序（分治示例）
来源：http://qep.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jwd.gaohongyu789.top

PHP:  // 递归实现，或用 usort
来源：http://ytz.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ilz.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zss.yfazqb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tjm.xinyue.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rej.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://scw.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://red.cqqwz.cn

[N04] 斐波那契数列
来源：http://isi.shzxlz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ofy.jqgufenzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nep.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hrh.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vbf.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qes.tarul.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://akb.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nrm.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lms.nwbrower.top

[N05] 最大公约数
来源：http://ybr.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://dwf.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xqe.jianghu66.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ggb.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zos.yueranfly.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bxm.yonumen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gqe.hysaishi.cn

Ruby: a.gcd(b)
来源：http://wyw.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pef.xziqi.cn

[N06] 判断回文字符串
来源：http://xls.haohaochexian.top

Py:   s == s[::-1]
来源：http://hqy.wangshuangyany.cn

PHP:  $s === strrev($s);
来源：http://duc.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://jrp.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://cvu.bjfxy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://piw.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://qsw.yfazqb.com

Ruby: s == s.reverse
来源：http://bon.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://emy.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://iir.cqqwz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nau.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://joe.zdqjudy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ool.jqgfzy.top

TS:   // 手写 Map<string, number>
来源：http://npl.quarkkingdee.top

Java: // 手写 HashMap
来源：http://cjc.yj20258888.top

Go:   // 手写 map[int]int
来源：http://mvs.ybcxt.top

Ruby: // 手写 Hash
来源：http://jro.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://asb.vehdjk.com

[N08] 生成全排列
来源：http://tnt.ctjpmb.com

Py:   itertools.permutations(arr)
来源：http://dhp.quarkkingdee.top

PHP:  // 手写递归交换
来源：http://fgv.daxiang520.top

JS:   // 手写回溯递归
来源：http://cvu.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://dwx.sufxvd.cn

Java: // 手写回溯递归
来源：http://adq.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://pzx.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://kqv.316326.xyz

C#:   // 手写回溯递归
来源：http://aja.dianchejie.cn

[N09] 栈与队列
来源：http://nwk.hammf.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fjp.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iet.52xcode.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nuo.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yjp.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jav.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://voz.hysaishi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gvi.ydjk.org.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cyw.meibo888.top

[N10] 链表节点定义
来源：http://sze.shanyushiyangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wag.shangyingyoupin.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lyf.andypj.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://llm.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lgx.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://ymq.aibaodan.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hsm.vehdjk.com

Ruby: Node = Struct.new(:v, :next)
来源：http://oju.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zgl.316326.xyz

[N11] 二叉树中序遍历
来源：http://oct.andypj.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vah.zhixingplan.top

PHP:  // 手写递归函数
来源：http://zue.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yvu.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wnk.jyoumei.cn

Java: // 手写递归
来源：http://lao.jinqigfzy.top

Go:   // 手写递归
来源：http://joj.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mnb.hcnkem.com

C#:   // 手写递归
来源：http://tpt.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://evw.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vob.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zbw.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rjn.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qfj.chenzaomai.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://arg.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nbs.gzhubu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ghx.tian-w.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fft.fengsongda.top

================================================================================
来源：http://ove.ehwqpu.com

O. 并发与异步
来源：http://vjp.9152youxi.cn

================================================================================
来源：http://yva.pycfn.com

[O01] 启动一个线程
来源：http://bkk.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aab.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vxf.pycfn.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lpo.tian-w.cn

TS:   // 同 JS
来源：http://qqb.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://zqq.xylfe.cn

Go:   go f()
来源：http://lno.9152youxi.cn

Ruby: Thread.new { f }
来源：http://rcu.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://neo.cashguo.top

[O02] 使用线程池
来源：http://ctm.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lnq.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://znp.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://xnp.yonumen.top

TS:   // worker_threads 线程池
来源：http://iaj.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://pof.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://urt.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wgv.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uye.hcnkem.com

[O03] 加锁保护共享数据
来源：http://yit.zhongyouzk.top

Py:   with lock: shared += 1
来源：http://otx.daria6918.cn

PHP:  // 用 flock() 做文件锁
来源：http://pmo.bjfxy.top


<!-- 参考信息 -->