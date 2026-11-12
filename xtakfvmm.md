代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ebh.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uyr.xuetiantiany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dzf.shangyingyoupin.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fht.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ryc.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pbw.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://hdy.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://yjw.kuanghao11.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bsi.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://dxm.fzhhl.top

TS:   v8.serialize(obj)        // Node
来源：http://pyt.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gkp.cdnleiting.top

Go:   encoding/gob
来源：http://jnt.andypj.xyz

Ruby: Marshal.dump(obj)
来源：http://xnu.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kas.fehbvm.com

================================================================================
来源：http://nsb.yuanzhike.top

L. 网络请求
来源：http://heg.cucudq.cn

================================================================================
来源：http://inc.jianghu66.top

[L01] 发送 GET 请求
来源：http://aqz.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ido.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://omt.zycfv.cn

JS:   await fetch(url)
来源：http://fle.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://kxz.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ylj.jyoumei.cn

Go:   resp, err := http.Get(url)
来源：http://sks.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wtt.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pnh.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://hfb.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://shq.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ilp.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ppp.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uue.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nqu.xingfuxueyuan.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jyf.fzhhl.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fss.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yui.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://rlk.guannengcc.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://acg.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xev.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://frs.316326.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wxs.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fpo.shuidangran.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://svh.ehwqpu.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fuv.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pjb.ydjk.org.cn

[L04] 设置超时
来源：http://ymh.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://pnt.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jye.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kxw.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mon.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bmf.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dro.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sgn.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mxd.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://wmf.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vzf.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tdn.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ltw.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fgs.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xwm.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xwz.hammf.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sao.zhaomingkeji.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hfm.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://xvm.sweek.top

Py:   resp.json()
来源：http://tcr.fengsongda.top

PHP:  json_decode($body, true);
来源：http://zjv.yvedp.cn

JS:   await resp.json()
来源：http://ydj.epnwcf.com

TS:   await resp.json()
来源：http://dxa.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tsu.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oru.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://xem.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vjx.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://pby.yuxming.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fch.chenjidiqi.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ysv.zdqjudy.top

JS:   resp.ok;  resp.status
来源：http://gwk.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://xvf.cashguo.top

Java: resp.statusCode()
来源：http://zju.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://lgs.sysykeji.top

Ruby: resp.code.to_i
来源：http://cku.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://tcd.52xcode.cn

[L08] 并发请求多个地址
来源：http://ols.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wzu.yanxiufei.cn

PHP:  curl_multi_init() 系列
来源：http://ehm.meibo888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jyz.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zsw.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qqi.ppjwa.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ugg.ydjk.org.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dlz.wangdashe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lxn.jinqigfzy.top

================================================================================
来源：http://rzd.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://fcb.cqqwz.cn

================================================================================
来源：http://dyz.fzhhl.top

[M01] 读取命令行参数
来源：http://bdy.tarul.cn

Py:   sys.argv[1:]
来源：http://nrp.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://okc.epnwcf.com

JS:   process.argv.slice(2)
来源：http://vlb.fzhhl.top

TS:   process.argv.slice(2)
来源：http://ekz.zhiwuduotai.top

Java: args 数组（main 方法参数）
来源：http://vlj.quarkkingdee.top

Go:   os.Args[1:]
来源：http://mzn.yvedp.cn

Ruby: ARGV
来源：http://ilz.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://tok.andypj.xyz

[M02] 读取环境变量
来源：http://wej.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://bzq.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hsr.0kj1m.cn

JS:   process.env.HOME
来源：http://fgj.cheryme.top

TS:   process.env.HOME
来源：http://ven.epnwcf.com

Java: System.getenv("HOME")
来源：http://cko.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://roj.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://cck.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tmh.hammf.cn

[M03] 执行外部命令
来源：http://qbe.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bih.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vbz.jlsjyb.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dik.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://vjj.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dzc.yueranfly.top

Go:   exec.Command("ls", "-l").Output()
来源：http://sjj.zhixingplan.top

Ruby: system("ls -l");  `ls -l`
来源：http://hew.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://vpv.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://lnj.daria6918.cn

Py:   os.getcwd()
来源：http://ory.zhengqikj.top

PHP:  getcwd();
来源：http://eyf.tianlin.xyz

JS:   process.cwd()
来源：http://duz.epnwcf.com

TS:   process.cwd()
来源：http://atr.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://qad.feifeiyinyue.top

Go:   os.Getwd()
来源：http://rag.fktsv.cn

Ruby: Dir.pwd
来源：http://nsi.vehdjk.com

C#:   Directory.GetCurrentDirectory()
来源：http://pxw.tian-w.cn

[M05] 设置退出码
来源：http://qgh.chenlongwang.top

Py:   sys.exit(1)
来源：http://eff.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://zea.dashuyun.cn

JS:   process.exit(1)
来源：http://bya.guannengcc.top

TS:   process.exit(1)
来源：http://tfv.yuanzhike.top

Java: System.exit(1)
来源：http://urr.nanxuanxn.top

Go:   os.Exit(1)
来源：http://xco.mhx1999.top

Ruby: exit 1
来源：http://fyx.jiagoushi.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ecd.guannengcc.top

[M06] 向标准错误输出
来源：http://csq.yangfankeji.com

Py:   print("err", file=sys.stderr)
来源：http://och.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://gfj.0kj1m.cn

JS:   console.error("err")
来源：http://zou.cqqwz.cn

TS:   console.error("err")
来源：http://eye.pengpengdd.cyou

Java: System.err.println("err")
来源：http://oyn.hfpthk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ygy.yangfankeji.com

Ruby: warn "err"
来源：http://pmi.xylfe.cn

C#:   Console.Error.WriteLine("err")
来源：http://eia.aibaodan.cn

[M07] 判断是否为主入口
来源：http://lwm.xziqi.cn

Py:   if __name__ == "__main__":
来源：http://mll.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uye.ydjk.org.cn

JS:   require.main === module
来源：http://cmb.ctjpmb.com

TS:   require.main === module
来源：http://wea.bjfxy.top

Java: public static void main(String[] args)
来源：http://nav.zhongyouzk.top

Go:   func main()
来源：http://mmq.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pww.yfazqb.com

C#:   static void Main(string[] args)
来源：http://fun.ivvv.top

[M08] 获取系统与运行时信息
来源：http://yga.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://qgx.jinqigfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://new.redwolf501.top

JS:   process.platform;  process.version
来源：http://fyl.guowangkeji.top

TS:   process.platform;  process.version
来源：http://mov.jinqigfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://meg.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kns.zhixingplan.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rbw.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://rja.svipenyu.cn

================================================================================
来源：http://lmp.nwbrower.top

N. 数据结构与算法
来源：http://mjw.jinyuanbaomall.cn

================================================================================
来源：http://oey.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://pnm.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eqo.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gjx.shuidangran.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uga.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jet.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://tvb.ywan-chungtsiang.top

Go:   sort.SearchInts(arr, x)
来源：http://epl.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jfr.pycfn.com

C#:   Array.BinarySearch(arr, x)
来源：http://eke.52xcode.cn

[N02] 排序（工程实践用内置实现）
来源：http://yrn.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://agk.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qbi.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gyy.hnqzz.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kjr.guowangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://esh.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://pgw.tanke756.top

Ruby: arr.sort
来源：http://pxg.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://iqi.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://use.wangdashe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eqf.haohaochexian.top

PHP:  // 递归实现，或用 usort
来源：http://ghe.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aiw.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fbx.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gaf.jinyuanbaomall.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://izk.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xfj.jlsjyb.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gos.cheryme.top

[N04] 斐波那契数列
来源：http://fmu.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dee.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xya.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://efz.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://duv.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dkd.cqqwz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xud.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fln.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gxx.sysykeji.top

[N05] 最大公约数
来源：http://ckl.hammf.cn

Py:   math.gcd(a, b)
来源：http://znl.hnxiangtu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zxo.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://boh.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iaj.hesvh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ufx.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jce.dashuyun.cn

Ruby: a.gcd(b)
来源：http://aum.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vsg.shuidangran.top

[N06] 判断回文字符串
来源：http://lfl.bjfxy.top

Py:   s == s[::-1]
来源：http://bcl.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://hed.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://bwz.jiagoushi.top

TS:   s === [...s].reverse().join("")
来源：http://mmx.yj202588.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nwu.c1oappe.top

Go:   // 双指针从两端比较
来源：http://jur.fzhhl.top

Ruby: s == s.reverse
来源：http://pzs.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jme.jinghuilouyu.cn

[N07] 两数之和（返回下标）
来源：http://tzy.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zqj.cdnleiting.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tpl.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oob.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://fut.cqqwz.cn

Java: // 手写 HashMap
来源：http://uzu.vehdjk.com

Go:   // 手写 map[int]int
来源：http://gbg.jinyuanbaomall.cn

Ruby: // 手写 Hash
来源：http://coi.cucudq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://luq.gaohongyu789.top

[N08] 生成全排列
来源：http://quc.cashguo.top

Py:   itertools.permutations(arr)
来源：http://nxn.jinqigufen.top

PHP:  // 手写递归交换
来源：http://ayh.fehbvm.com

JS:   // 手写回溯递归
来源：http://gjt.ivvv.top

TS:   // 手写回溯递归
来源：http://zty.tianlin.xyz

Java: // 手写回溯递归
来源：http://ypd.aizwys.cn

Go:   // 手写回溯递归
来源：http://crh.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://lvb.tianlin.xyz

C#:   // 手写回溯递归
来源：http://cgr.tian-w.cn

[N09] 栈与队列
来源：http://zyu.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://duq.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ajb.hysaishi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zyx.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ria.hesvh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xbn.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nxi.316326.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hrp.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fxu.tanke756.top

[N10] 链表节点定义
来源：http://fln.ybcxt.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sob.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://auk.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vqt.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mhe.meibo888.top

Java: class Node { int v; Node next; }
来源：http://hzl.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://xhy.cdnleiting.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gze.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://kqn.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://opj.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://keh.sjlbkw.cn

PHP:  // 手写递归函数
来源：http://yft.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://esj.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pqc.316326.xyz

Java: // 手写递归
来源：http://tym.gaohongyu789.top

Go:   // 手写递归
来源：http://arj.jianghu66.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lyx.gaohongyu789.top

C#:   // 手写递归
来源：http://fht.zdbjq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pnc.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://upk.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jdw.jiagoushi.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rky.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dwy.chenjidiqi.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iio.wangshuangyany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ftt.nanxinkj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bio.yanxiufei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gbp.snrcjt.cn

================================================================================
来源：http://kyx.hesvh.cn

O. 并发与异步
来源：http://uii.hongshengwenyu.top

================================================================================
来源：http://grl.xziqi.cn

[O01] 启动一个线程
来源：http://rzd.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uem.c1oappe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pax.andypj.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://haz.yongpay.top

TS:   // 同 JS
来源：http://qsf.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://jzi.feifeiyinyue.top

Go:   go f()
来源：http://ogz.yonumen.top

Ruby: Thread.new { f }
来源：http://ngt.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://edf.yj20258.top

[O02] 使用线程池
来源：http://rtu.epnwcf.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://djl.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ejn.fanxiaobao.xyz

JS:   // worker_threads 线程池
来源：http://ato.ehwqpu.com

TS:   // worker_threads 线程池
来源：http://qhy.havefunace.top

Java: Executors.newFixedThreadPool(4)
来源：http://gmp.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nkq.shuidangran.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ygq.sjlbkw.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://csf.gotoacloud.top

[O03] 加锁保护共享数据
来源：http://yuy.316326.xyz

Py:   with lock: shared += 1
来源：http://kqa.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://luj.tian-w.cn


<!-- 参考信息 -->