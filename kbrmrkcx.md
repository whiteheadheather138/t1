代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uhn.zhaomingkeji.xyz

[K07] 进制转换
来源：http://hdb.wangdashe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gvh.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://amc.zhoulong.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dhd.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lbc.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dfw.xuetiantiany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ebg.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ejo.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pff.yueranfly.top

[K08] 二进制序列化（非 JSON）
来源：http://fiy.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://aob.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://peg.tanke756.top

JS:   v8.serialize(obj)        // Node
来源：http://wpy.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://spy.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tqx.shanyushiyangtech.top

Go:   encoding/gob
来源：http://aug.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://yml.ivvv.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bmy.jlsjyb.cn

================================================================================
来源：http://lah.chenjidiqi.icu

L. 网络请求
来源：http://xpg.dianchejie.cn

================================================================================
来源：http://oop.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://tgb.jinqigufen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fox.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vxx.fzhhl.top

JS:   await fetch(url)
来源：http://rbo.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://pud.uphjek.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wbf.pengpengdd.cyou

Go:   resp, err := http.Get(url)
来源：http://qxe.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qie.fktsv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zhr.tianlin.xyz

[L02] 发送 POST JSON
来源：http://fxs.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://yaq.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://emr.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bas.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oow.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fgk.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pek.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kbg.snrcjt.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yee.chenlongwang.top

[L03] 设置自定义请求头
来源：http://nyf.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kob.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ixl.jyoumei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zjs.hywenlv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zfx.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cfx.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aey.pengpengdd.cyou

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://joe.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aqw.bjfxy.top

[L04] 设置超时
来源：http://buu.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://qmu.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eqr.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wds.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://irj.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://drg.hongshengwenyu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cfy.xingfuxueyuan.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nte.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wrl.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://fid.zhixingplan.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mhe.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xmn.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zbc.fengsongda.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bkz.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hdl.hywenlv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oez.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ojj.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dyt.yvedp.cn

[L06] 解析响应为 JSON
来源：http://rlx.fengsongda.top

Py:   resp.json()
来源：http://wwa.yfazqb.com

PHP:  json_decode($body, true);
来源：http://yhd.guannengcc.top

JS:   await resp.json()
来源：http://yer.wangdashe.top

TS:   await resp.json()
来源：http://wxx.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hhc.tanke756.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rbs.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://jcd.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fkh.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://wvh.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wkz.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://glv.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://nrl.zhaomingkeji.xyz

TS:   resp.ok;  resp.status
来源：http://fdm.zhixingplan.top

Java: resp.statusCode()
来源：http://mdl.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://vnj.jiagoushi.top

Ruby: resp.code.to_i
来源：http://kcx.jinghuilouyu.cn

C#:   (int)resp.StatusCode
来源：http://fhb.ydzc1.top

[L08] 并发请求多个地址
来源：http://eyn.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vrd.jianghu66.top

PHP:  curl_multi_init() 系列
来源：http://icc.xuanzx.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tro.sjlbkw.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ksx.0kj1m.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hff.zhengqikj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yqp.uphjek.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://paw.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dqv.fktsv.cn

================================================================================
来源：http://fna.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://znd.cucudq.cn

================================================================================
来源：http://etm.zhiwuduotai.top

[M01] 读取命令行参数
来源：http://syz.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://efa.yfazqb.com

PHP:  $argv;  $argc;
来源：http://zwl.jqgufenzy.top

JS:   process.argv.slice(2)
来源：http://xfo.yj202588.top

TS:   process.argv.slice(2)
来源：http://msl.ydjk.org.cn

Java: args 数组（main 方法参数）
来源：http://yed.iojbl.cn

Go:   os.Args[1:]
来源：http://lrk.hywenlv.cn

Ruby: ARGV
来源：http://ftd.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://vvx.jinqigufen.top

[M02] 读取环境变量
来源：http://gtv.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://twj.9152youxi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://taf.xylfe.cn

JS:   process.env.HOME
来源：http://zsc.zhixingplan.top

TS:   process.env.HOME
来源：http://kba.ybcxt.top

Java: System.getenv("HOME")
来源：http://prx.dashuyun.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aky.haohaochexian.top

Ruby: ENV["HOME"]
来源：http://tyh.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aam.nwbrower.top

[M03] 执行外部命令
来源：http://vxw.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mwg.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gxp.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nid.quarkkingdee.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hwu.zhijiandao.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bxj.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zez.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://ynl.zhongyouzk.top

C#:   Process.Start("ls", "-l");
来源：http://avn.cucudq.cn

[M04] 获取当前工作目录
来源：http://hyz.ivvv.top

Py:   os.getcwd()
来源：http://rqb.wangdashe.top

PHP:  getcwd();
来源：http://bky.zhixingplan.top

JS:   process.cwd()
来源：http://jfu.yangfankeji.com

TS:   process.cwd()
来源：http://woq.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://nhi.fanxiaobao.xyz

Go:   os.Getwd()
来源：http://fsg.yongpay.top

Ruby: Dir.pwd
来源：http://bem.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://bre.shanyushiyangtech.top

[M05] 设置退出码
来源：http://mgt.vqdsnc.cn

Py:   sys.exit(1)
来源：http://nwa.hammf.cn

PHP:  exit(1);
来源：http://ztf.hesvh.cn

JS:   process.exit(1)
来源：http://nya.hysaishi.cn

TS:   process.exit(1)
来源：http://oyo.havefunace.top

Java: System.exit(1)
来源：http://hwd.dianchejie.cn

Go:   os.Exit(1)
来源：http://sgd.ppjwa.cn

Ruby: exit 1
来源：http://stq.ydjk.org.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mth.mhx1999.top

[M06] 向标准错误输出
来源：http://pxv.meibo888.top

Py:   print("err", file=sys.stderr)
来源：http://mpz.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nqh.zhoulong.xyz

JS:   console.error("err")
来源：http://ida.gogol.net.cn

TS:   console.error("err")
来源：http://lox.daxiang520.top

Java: System.err.println("err")
来源：http://noc.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://krv.zhoulong.xyz

Ruby: warn "err"
来源：http://voh.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://eft.zhengqikj.top

[M07] 判断是否为主入口
来源：http://iff.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://meg.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zaa.vehdjk.com

JS:   require.main === module
来源：http://dca.smart0.xyz

TS:   require.main === module
来源：http://stz.xziqi.cn

Java: public static void main(String[] args)
来源：http://lhn.cashguo.top

Go:   func main()
来源：http://jrl.hysaishi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://stz.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://uek.daxiang520.top

[M08] 获取系统与运行时信息
来源：http://ize.gzhubu.top

Py:   platform.system();  platform.python_version()
来源：http://lfn.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://fzk.zdbjq.cn

JS:   process.platform;  process.version
来源：http://qth.hcnkem.com

TS:   process.platform;  process.version
来源：http://qnf.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://phy.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ocf.ehwqpu.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ven.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hjn.zycfv.cn

================================================================================
来源：http://gjs.tian-w.cn

N. 数据结构与算法
来源：http://lbn.hysaishi.cn

================================================================================
来源：http://whb.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://qho.haohaochexian.top

Py:   bisect.bisect_left(arr, x)
来源：http://kui.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wkq.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fso.kuanghao11.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zeq.bjfxy.top

Java: Arrays.binarySearch(arr, x)
来源：http://evq.hammf.cn

Go:   sort.SearchInts(arr, x)
来源：http://wmz.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rgz.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://jbj.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://unq.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://bug.shzxlz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cxy.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yut.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cvn.zhoulong.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jep.uphjek.com

Go:   slices.Sort(arr)
来源：http://drq.zhongyouzk.top

Ruby: arr.sort
来源：http://bcz.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fbd.gaohongyu789.top

[N03] 快速排序（分治示例）
来源：http://rru.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jzm.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://woi.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://grt.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pju.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ajj.fanxiaobao.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dfv.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qig.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://mdn.iojbl.cn

[N04] 斐波那契数列
来源：http://knj.aibaodan.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yse.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ovn.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oyv.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wml.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://paf.yanxiufei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ygv.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sla.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xnk.haohaochexian.top

[N05] 最大公约数
来源：http://fkk.jlsjyb.cn

Py:   math.gcd(a, b)
来源：http://ynh.nanxinkj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mid.hnxiangtu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hax.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vis.haohaochexian.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zkw.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ovj.yuanzhike.top

Ruby: a.gcd(b)
来源：http://yxd.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uni.ppjwa.cn

[N06] 判断回文字符串
来源：http://lvy.daxiang520.top

Py:   s == s[::-1]
来源：http://ysx.dianchejie.cn

PHP:  $s === strrev($s);
来源：http://dly.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://vdz.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://cvp.sufxvd.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kgx.svipenyu.cn

Go:   // 双指针从两端比较
来源：http://ytc.guowangkeji.top

Ruby: s == s.reverse
来源：http://yqs.jinyuanbaomall.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bso.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://jko.yanxiufei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wtk.havefunace.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bhf.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nno.jyoumei.cn

TS:   // 手写 Map<string, number>
来源：http://ath.tian-w.cn

Java: // 手写 HashMap
来源：http://sql.ydjk.org.cn

Go:   // 手写 map[int]int
来源：http://ckh.smart0.xyz

Ruby: // 手写 Hash
来源：http://gyo.yvedp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fyl.gogol.net.cn

[N08] 生成全排列
来源：http://qpx.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://ejo.tianlin.xyz

PHP:  // 手写递归交换
来源：http://rzz.smart0.xyz

JS:   // 手写回溯递归
来源：http://lvp.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://kse.aibaodan.cn

Java: // 手写回溯递归
来源：http://jut.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://jic.yj202588.top

Ruby: arr.permutation.to_a
来源：http://gzq.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://umo.52xcode.cn

[N09] 栈与队列
来源：http://rlc.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ybf.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://itm.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://avu.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vny.xziqi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mwo.yuxming.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mmm.epnwcf.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yex.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mge.nanxinkj.top

[N10] 链表节点定义
来源：http://now.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://odl.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kcl.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://spx.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vsh.yj20258.top

Java: class Node { int v; Node next; }
来源：http://rkf.hnqzz.top

Go:   type Node struct { V int; Next *Node }
来源：http://uom.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fyr.yuxming.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ocr.cashguo.top

[N11] 二叉树中序遍历
来源：http://ple.hammf.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hap.xuanzx.com

PHP:  // 手写递归函数
来源：http://lzn.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kqu.shangyingyoupin.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://icw.epnwcf.com

Java: // 手写递归
来源：http://auy.pengpengdd.cyou

Go:   // 手写递归
来源：http://xws.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://epy.yangfankeji.com

C#:   // 手写递归
来源：http://yuj.fzhhl.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mox.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://liu.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oim.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ksd.svipenyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bbu.jinghuilouyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hir.jyoumei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cxi.andypj.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tox.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mgg.hfpthk.cn

================================================================================
来源：http://ifa.fanxiaobao.xyz

O. 并发与异步
来源：http://azp.smart0.xyz

================================================================================
来源：http://nuc.nanxuanxn.top

[O01] 启动一个线程
来源：http://xqj.jinyuanbaomall.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kxq.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mkh.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qez.zhixingplan.top

TS:   // 同 JS
来源：http://rez.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://pop.cucudq.cn

Go:   go f()
来源：http://edy.cashguo.top

Ruby: Thread.new { f }
来源：http://sfw.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://kxy.jinqigfzy.top

[O02] 使用线程池
来源：http://khe.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mpc.hnxiangtu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vyv.cashguo.top

JS:   // worker_threads 线程池
来源：http://kfx.pycfn.com

TS:   // worker_threads 线程池
来源：http://xlj.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://nyi.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://krm.aizwys.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yxf.jqgfzy.top


<!-- 参考信息 -->