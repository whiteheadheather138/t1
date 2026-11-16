代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jjv.aizwys.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fik.uphjek.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pqq.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xos.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nni.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hju.tianlin.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ffs.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://opx.hfpthk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lln.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://ong.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://opp.zdbjq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://znn.hesvh.cn

Go:   encoding/gob
来源：http://tla.smart0.xyz

Ruby: Marshal.dump(obj)
来源：http://yxq.dashuyun.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cbd.yanxiufei.cn

================================================================================
来源：http://tor.gotoacloud.top

L. 网络请求
来源：http://qgj.hammf.cn

================================================================================
来源：http://djn.jyoumei.cn

[L01] 发送 GET 请求
来源：http://eqd.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://azm.hywenlv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xir.hcnkem.com

JS:   await fetch(url)
来源：http://szt.birdmap.top

TS:   await fetch(url)
来源：http://mnd.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kgq.iojbl.cn

Go:   resp, err := http.Get(url)
来源：http://hbz.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ryi.fanxiaobao.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yyv.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://ynp.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://puc.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zei.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rye.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sca.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fdi.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oxk.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aav.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dbm.birdmap.top

[L03] 设置自定义请求头
来源：http://irt.svipenyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sxy.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kor.yangfankeji.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gqb.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jwk.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://omj.jinghuilouyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ioo.aibaodan.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yea.xziqi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zbz.cucudq.cn

[L04] 设置超时
来源：http://rhx.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://rzw.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ilp.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zyi.jinyuanbaomall.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://icl.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gel.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eig.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kdq.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fxa.smart0.xyz

[L05] 上传文件（multipart）
来源：http://xzg.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lie.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://syz.316326.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mjj.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dzz.fehbvm.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blz.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hmp.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nas.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pgs.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://kuo.xuetiantiany.cn

Py:   resp.json()
来源：http://anm.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://nnb.daxiang520.top

JS:   await resp.json()
来源：http://jmn.iojbl.cn

TS:   await resp.json()
来源：http://rrf.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yhj.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lrv.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://kym.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xoc.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://cxq.sysykeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ttw.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bkk.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://kdz.fzhhl.top

TS:   resp.ok;  resp.status
来源：http://yxk.yangfankeji.com

Java: resp.statusCode()
来源：http://qff.ctjpmb.com

Go:   resp.StatusCode
来源：http://aum.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://fjj.316326.xyz

C#:   (int)resp.StatusCode
来源：http://tyh.kuanghao11.cn

[L08] 并发请求多个地址
来源：http://lcg.ehwqpu.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ycu.hnxiangtu.top

PHP:  curl_multi_init() 系列
来源：http://bfu.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lmu.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lze.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nye.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pdv.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nvv.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iru.birdmap.top

================================================================================
来源：http://emc.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://ihn.jiagoushi.top

================================================================================
来源：http://xhj.xziqi.cn

[M01] 读取命令行参数
来源：http://mmb.nanxinkj.top

Py:   sys.argv[1:]
来源：http://mix.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://mxz.dashuyun.cn

JS:   process.argv.slice(2)
来源：http://peg.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://gje.ivvv.top

Java: args 数组（main 方法参数）
来源：http://aet.chenzaomai.com

Go:   os.Args[1:]
来源：http://lmr.ybcxt.top

Ruby: ARGV
来源：http://tyw.tarul.cn

C#:   args 数组（Main 方法参数）
来源：http://ajk.jinqigfzy.top

[M02] 读取环境变量
来源：http://nno.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://ubu.hesvh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rlu.jqgfzy.top

JS:   process.env.HOME
来源：http://gog.hcnkem.com

TS:   process.env.HOME
来源：http://qbw.yongpay.top

Java: System.getenv("HOME")
来源：http://ztx.daria6918.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lzn.hesvh.cn

Ruby: ENV["HOME"]
来源：http://lhn.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ofg.bjfxy.top

[M03] 执行外部命令
来源：http://lzs.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mai.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://brp.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://hrf.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wvk.feifeiyinyue.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gpl.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ano.ywan-chungtsiang.top

Ruby: system("ls -l");  `ls -l`
来源：http://ldd.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://ttb.cashguo.top

[M04] 获取当前工作目录
来源：http://upl.havefunace.top

Py:   os.getcwd()
来源：http://ttr.jinqigufen.top

PHP:  getcwd();
来源：http://jvb.nanxuanxn.top

JS:   process.cwd()
来源：http://nuz.fanxiaobao.xyz

TS:   process.cwd()
来源：http://jch.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://apl.jyoumei.cn

Go:   os.Getwd()
来源：http://fsn.hcnkem.com

Ruby: Dir.pwd
来源：http://ikp.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ymw.ydjk.org.cn

[M05] 设置退出码
来源：http://psm.zhijiandao.cn

Py:   sys.exit(1)
来源：http://voq.316326.xyz

PHP:  exit(1);
来源：http://apu.hcnkem.com

JS:   process.exit(1)
来源：http://com.zhongyouzk.top

TS:   process.exit(1)
来源：http://mya.yueranfly.top

Java: System.exit(1)
来源：http://uox.zdbjq.cn

Go:   os.Exit(1)
来源：http://uey.nwbrower.top

Ruby: exit 1
来源：http://fpm.dianchejie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vxc.52xcode.cn

[M06] 向标准错误输出
来源：http://prp.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://lfo.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ipa.iojbl.cn

JS:   console.error("err")
来源：http://kfr.yonumen.top

TS:   console.error("err")
来源：http://kmc.nwbrower.top

Java: System.err.println("err")
来源：http://snz.quarkkingdee.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dqp.iojbl.cn

Ruby: warn "err"
来源：http://kgi.0kj1m.cn

C#:   Console.Error.WriteLine("err")
来源：http://rwu.zdbjq.cn

[M07] 判断是否为主入口
来源：http://oem.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://iyk.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iem.ivvv.top

JS:   require.main === module
来源：http://ssi.yangfankeji.com

TS:   require.main === module
来源：http://zeh.cashguo.top

Java: public static void main(String[] args)
来源：http://ttq.hywenlv.cn

Go:   func main()
来源：http://rhm.tianlin.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://civ.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://hsj.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://rwh.jqgufenzy.top

Py:   platform.system();  platform.python_version()
来源：http://skt.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://zto.fktsv.cn

JS:   process.platform;  process.version
来源：http://ygg.bbcook.cn

TS:   process.platform;  process.version
来源：http://txr.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yix.yj20258.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ymr.fehbvm.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fng.xylfe.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bxq.yuxming.cn

================================================================================
来源：http://jri.zhengqikj.top

N. 数据结构与算法
来源：http://piq.quarkkingdee.top

================================================================================
来源：http://den.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://mws.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nia.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xim.gogol.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hwb.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://chi.bbcook.cn

Java: Arrays.binarySearch(arr, x)
来源：http://edl.gogol.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://csb.cqqwz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tsr.hammf.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lub.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://fet.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://iri.shzxlz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qqy.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://njo.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vcd.haohaochexian.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xky.ctjpmb.com

Go:   slices.Sort(arr)
来源：http://etu.yj20258.top

Ruby: arr.sort
来源：http://jsp.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://efy.yj20258888.top

[N03] 快速排序（分治示例）
来源：http://wkg.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jrd.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://uob.fktsv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tcn.jinqigufen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://byk.jianghu66.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vhk.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eym.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dzk.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ybl.nwbrower.top

[N04] 斐波那契数列
来源：http://ujr.52xcode.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://war.xinyue.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qrf.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ybz.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blu.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mkf.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lrh.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jcq.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vtt.ywan-chungtsiang.top

[N05] 最大公约数
来源：http://uek.cashguo.top

Py:   math.gcd(a, b)
来源：http://eqc.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sri.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uoe.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://roc.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://abp.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vqm.cheryme.top

Ruby: a.gcd(b)
来源：http://ilv.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nmp.zhongyouzk.top

[N06] 判断回文字符串
来源：http://xob.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://lbp.dianchejie.cn

PHP:  $s === strrev($s);
来源：http://vgy.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://sde.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://rsz.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ibs.uphjek.com

Go:   // 双指针从两端比较
来源：http://kvx.dianchejie.cn

Ruby: s == s.reverse
来源：http://kag.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gke.mhx1999.top

[N07] 两数之和（返回下标）
来源：http://pqr.jyoumei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://twp.cashguo.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bsm.jyoumei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nfj.gotoacloud.top

TS:   // 手写 Map<string, number>
来源：http://ycg.tianlin.xyz

Java: // 手写 HashMap
来源：http://kzw.yfazqb.com

Go:   // 手写 map[int]int
来源：http://aql.hfpthk.cn

Ruby: // 手写 Hash
来源：http://use.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xmx.shangyingyoupin.top

[N08] 生成全排列
来源：http://zev.hnqzz.top

Py:   itertools.permutations(arr)
来源：http://wxe.uphjek.com

PHP:  // 手写递归交换
来源：http://wjw.ppjwa.cn

JS:   // 手写回溯递归
来源：http://cem.ehwqpu.com

TS:   // 手写回溯递归
来源：http://mez.dianchejie.cn

Java: // 手写回溯递归
来源：http://pdf.yonumen.top

Go:   // 手写回溯递归
来源：http://gcp.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://xpu.shanyushiyangtech.top

C#:   // 手写回溯递归
来源：http://ydw.zycfv.cn

[N09] 栈与队列
来源：http://bib.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yzy.zhoulong.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qcs.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xzj.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hik.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ypv.hcnkem.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://emf.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rbg.ydzc1.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tkv.ehwqpu.com

[N10] 链表节点定义
来源：http://idm.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fzs.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hlw.gogol.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dbo.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nfk.ywan-chungtsiang.top

Java: class Node { int v; Node next; }
来源：http://teq.shuidangran.top

Go:   type Node struct { V int; Next *Node }
来源：http://xwu.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wyi.yanxiufei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xqt.ybcxt.top

[N11] 二叉树中序遍历
来源：http://uso.svipenyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://erm.wangdashe.top

PHP:  // 手写递归函数
来源：http://czy.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fpf.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cde.jinqigfzy.top

Java: // 手写递归
来源：http://ctr.gogol.net.cn

Go:   // 手写递归
来源：http://lzt.birdmap.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ntv.kuanghao11.cn

C#:   // 手写递归
来源：http://uvf.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rdf.fengsongda.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wyl.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fsq.jiagoushi.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xnd.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yrb.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ldb.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xkf.zhiwuduotai.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hfb.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cny.yfazqb.com

================================================================================
来源：http://nuv.hfpthk.cn

O. 并发与异步
来源：http://viq.shuidangran.top

================================================================================
来源：http://xva.cashguo.top

[O01] 启动一个线程
来源：http://kmi.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ipt.yvedp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gzf.cucudq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qud.svipenyu.cn

TS:   // 同 JS
来源：http://kro.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://xmz.shangyingyoupin.top

Go:   go f()
来源：http://wlr.sysykeji.top

Ruby: Thread.new { f }
来源：http://qir.yj20258.top

C#:   Task.Run(() => F());
来源：http://tan.nanxinkj.top

[O02] 使用线程池
来源：http://dyq.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pda.zdbjq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bie.nanxinkj.top

JS:   // worker_threads 线程池
来源：http://jxf.0kj1m.cn

TS:   // worker_threads 线程池
来源：http://opb.316326.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://kqh.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hmi.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xhh.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xio.tian-w.cn

[O03] 加锁保护共享数据
来源：http://uef.chenzaomai.com

Py:   with lock: shared += 1
来源：http://frw.tarul.cn

PHP:  // 用 flock() 做文件锁
来源：http://prj.hcnkem.com


<!-- 参考信息 -->