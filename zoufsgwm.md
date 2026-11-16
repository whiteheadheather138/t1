代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://aod.xinyue.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://sft.svipenyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wnl.shuidangran.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jxo.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://ufg.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gwt.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://gvw.wangshuangyany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://khq.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gqo.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ebx.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://epi.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://juc.andypj.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qdm.zhaomingkeji.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://epc.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kkk.shuidangran.top

[K05] 深拷贝对象
来源：http://fyj.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://phz.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://sqr.ydzc1.top

JS:   structuredClone(obj)
来源：http://ovr.fanxiaobao.xyz

TS:   structuredClone(obj)
来源：http://vxd.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rsr.0kj1m.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jcz.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qhm.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kaj.bjfxy.top

[K06] 解析 URL 查询串
来源：http://htr.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wdf.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://btt.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://luw.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ayu.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ula.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zyn.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bga.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pum.cashguo.top

[K07] 进制转换
来源：http://uew.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hkb.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rla.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lio.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vxf.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nps.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cba.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://adt.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ntb.aibaodan.cn

[K08] 二进制序列化（非 JSON）
来源：http://gvd.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://leo.zycfv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ybc.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://sda.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://tmc.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kta.dianchejie.cn

Go:   encoding/gob
来源：http://gto.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://fft.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dip.jqgufenzy.top

================================================================================
来源：http://xrw.cdnleiting.top

L. 网络请求
来源：http://rcn.sufxvd.cn

================================================================================
来源：http://klg.aibaodan.cn

[L01] 发送 GET 请求
来源：http://vrj.hcnkem.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://liu.sufxvd.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bwu.ybcxt.top

JS:   await fetch(url)
来源：http://afq.sufxvd.cn

TS:   await fetch(url)
来源：http://zng.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://chl.wangshuangyany.cn

Go:   resp, err := http.Get(url)
来源：http://wit.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://aya.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sxn.zhijiandao.cn

[L02] 发送 POST JSON
来源：http://zpo.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://scc.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xxp.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zwl.wangdashe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yms.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uor.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zod.shanyushiyangtech.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tox.aibaodan.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ngz.haohaochexian.top

[L03] 设置自定义请求头
来源：http://eok.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lxe.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wnm.sysykeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://onu.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ycp.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ysd.epnwcf.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fed.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://igb.yonumen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uot.pengpengdd.cyou

[L04] 设置超时
来源：http://zpn.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://khi.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yeg.tarul.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://izd.haohaochexian.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tgw.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bxf.vehdjk.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fco.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ogm.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vlu.ivvv.top

[L05] 上传文件（multipart）
来源：http://fio.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xev.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nmk.chenjidiqi.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wkb.gzhubu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vgz.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hyl.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xtr.guowangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cum.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rna.bbcook.cn

[L06] 解析响应为 JSON
来源：http://jbc.yuanzhike.top

Py:   resp.json()
来源：http://wku.c1oappe.top

PHP:  json_decode($body, true);
来源：http://fyc.jinghuilouyu.cn

JS:   await resp.json()
来源：http://cac.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://qqv.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lve.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ywa.shanyushiyangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://nte.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gml.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://jqw.jqgfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gqz.yueranfly.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uoz.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://vpf.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://qgo.xinyue.icu

Java: resp.statusCode()
来源：http://znu.yanxiufei.cn

Go:   resp.StatusCode
来源：http://dto.hcnkem.com

Ruby: resp.code.to_i
来源：http://tzp.316326.xyz

C#:   (int)resp.StatusCode
来源：http://ozo.sufxvd.cn

[L08] 并发请求多个地址
来源：http://ijk.jinyuanbaomall.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uya.sysykeji.top

PHP:  curl_multi_init() 系列
来源：http://igt.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zwi.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jwt.tanke756.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mgt.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gba.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cjd.chenlongwang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wtl.feifeiyinyue.top

================================================================================
来源：http://sta.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://xgz.quarkkingdee.top

================================================================================
来源：http://wiw.hammf.cn

[M01] 读取命令行参数
来源：http://nny.tanke756.top

Py:   sys.argv[1:]
来源：http://skg.hcnkem.com

PHP:  $argv;  $argc;
来源：http://jnw.9152youxi.cn

JS:   process.argv.slice(2)
来源：http://vsk.cashguo.top

TS:   process.argv.slice(2)
来源：http://laa.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://bqc.yuxming.cn

Go:   os.Args[1:]
来源：http://sfi.jinqigfzy.top

Ruby: ARGV
来源：http://xei.ywan-chungtsiang.top

C#:   args 数组（Main 方法参数）
来源：http://iov.daxiang520.top

[M02] 读取环境变量
来源：http://ajm.chenjidiqi.icu

Py:   os.environ.get("HOME")
来源：http://njn.shangyingyoupin.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://umo.ppjwa.cn

JS:   process.env.HOME
来源：http://fdy.zhijiandao.cn

TS:   process.env.HOME
来源：http://pjg.hammf.cn

Java: System.getenv("HOME")
来源：http://kko.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gjy.yuanzhike.top

Ruby: ENV["HOME"]
来源：http://rpj.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://psw.guowangkeji.top

[M03] 执行外部命令
来源：http://mps.andypj.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qfg.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gzs.sufxvd.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gky.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ewa.hysaishi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pwt.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mlz.iojbl.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wum.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://bxg.zhengqikj.top

[M04] 获取当前工作目录
来源：http://xxp.zycfv.cn

Py:   os.getcwd()
来源：http://xqm.tarul.cn

PHP:  getcwd();
来源：http://vqh.bbcook.cn

JS:   process.cwd()
来源：http://rij.0kj1m.cn

TS:   process.cwd()
来源：http://rxi.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://qsm.jiagoushi.top

Go:   os.Getwd()
来源：http://qoi.yvedp.cn

Ruby: Dir.pwd
来源：http://vxn.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://yza.52xcode.cn

[M05] 设置退出码
来源：http://eol.yvedp.cn

Py:   sys.exit(1)
来源：http://sot.cheryme.top

PHP:  exit(1);
来源：http://fti.xylfe.cn

JS:   process.exit(1)
来源：http://fxe.hesvh.cn

TS:   process.exit(1)
来源：http://lcv.hywenlv.cn

Java: System.exit(1)
来源：http://erw.yanxiufei.cn

Go:   os.Exit(1)
来源：http://wpk.ydjk.org.cn

Ruby: exit 1
来源：http://pwc.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mpq.tianlin.xyz

[M06] 向标准错误输出
来源：http://hjf.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://uej.hywenlv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rpu.epnwcf.com

JS:   console.error("err")
来源：http://bda.svipenyu.cn

TS:   console.error("err")
来源：http://esz.fengsongda.top

Java: System.err.println("err")
来源：http://zpj.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://frc.jyoumei.cn

Ruby: warn "err"
来源：http://ruz.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://igz.ybcxt.top

[M07] 判断是否为主入口
来源：http://szr.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://wln.wangdashe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tel.tianlin.xyz

JS:   require.main === module
来源：http://cmb.chenjidiqi.icu

TS:   require.main === module
来源：http://qys.sysykeji.top

Java: public static void main(String[] args)
来源：http://paf.sjlbkw.cn

Go:   func main()
来源：http://xfc.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://koi.hesvh.cn

C#:   static void Main(string[] args)
来源：http://hjx.yj20258.top

[M08] 获取系统与运行时信息
来源：http://tyi.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://kfw.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://vra.pengpengdd.cyou

JS:   process.platform;  process.version
来源：http://yii.hcnkem.com

TS:   process.platform;  process.version
来源：http://ftt.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ujy.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vct.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kco.bbcook.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vbk.yuxming.cn

================================================================================
来源：http://aqg.yj20258.top

N. 数据结构与算法
来源：http://akn.tianlin.xyz

================================================================================
来源：http://tkv.cucudq.cn

[N01] 二分查找（有序数组）
来源：http://svl.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xda.zhixingplan.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://icg.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hub.tian-w.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cbi.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://ojg.fehbvm.com

Go:   sort.SearchInts(arr, x)
来源：http://qzm.hnqzz.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xcw.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://wzy.yj20258888.top

[N02] 排序（工程实践用内置实现）
来源：http://eun.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://eov.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rqx.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://iox.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kqx.mhx1999.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://coc.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://egn.jianghu66.top

Ruby: arr.sort
来源：http://qqj.nanxuanxn.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nbf.daxiang520.top

[N03] 快速排序（分治示例）
来源：http://ctx.jianghu66.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ncd.tianlin.xyz

PHP:  // 递归实现，或用 usort
来源：http://fus.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hil.cqqwz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://laf.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://umb.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bzr.sweek.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gtz.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ifg.zhixingplan.top

[N04] 斐波那契数列
来源：http://ahq.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jln.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pui.dashuyun.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zjh.fehbvm.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bos.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mgp.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mei.gaohongyu789.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mfo.iojbl.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kad.fehbvm.com

[N05] 最大公约数
来源：http://tks.vehdjk.com

Py:   math.gcd(a, b)
来源：http://trr.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://drj.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://efo.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://det.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hsc.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://exn.cdnleiting.top

Ruby: a.gcd(b)
来源：http://ygk.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lch.yj20258888.top

[N06] 判断回文字符串
来源：http://isu.xinyue.icu

Py:   s == s[::-1]
来源：http://pnf.andypj.xyz

PHP:  $s === strrev($s);
来源：http://gyr.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://vvk.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://lbd.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xnc.zdbjq.cn

Go:   // 双指针从两端比较
来源：http://kxd.ybcxt.top

Ruby: s == s.reverse
来源：http://aeb.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xwg.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://ufu.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tqv.guannengcc.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kpn.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lyi.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://beh.hcnkem.com

Java: // 手写 HashMap
来源：http://jal.hammf.cn

Go:   // 手写 map[int]int
来源：http://zep.cdnleiting.top

Ruby: // 手写 Hash
来源：http://mjb.birdmap.top

C#:   // 手写 Dictionary<int, int>
来源：http://kbj.c1oappe.top

[N08] 生成全排列
来源：http://avu.cashguo.top

Py:   itertools.permutations(arr)
来源：http://bmj.jianghu66.top

PHP:  // 手写递归交换
来源：http://oeb.daria6918.cn

JS:   // 手写回溯递归
来源：http://zms.dianchejie.cn

TS:   // 手写回溯递归
来源：http://ovq.bjfxy.top

Java: // 手写回溯递归
来源：http://cov.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://kip.xylfe.cn

Ruby: arr.permutation.to_a
来源：http://qxk.jiagoushi.top

C#:   // 手写回溯递归
来源：http://guz.yangfankeji.com

[N09] 栈与队列
来源：http://ylt.gzhubu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ynu.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gxw.jqgufenzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eia.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://djf.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oqu.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://izs.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eid.dashuyun.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wgl.yj20258888.top

[N10] 链表节点定义
来源：http://jqq.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://roj.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sic.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kaq.ydzc1.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aoh.gaohongyu789.top

Java: class Node { int v; Node next; }
来源：http://tvp.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://wvz.gzhubu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jro.xylfe.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kjs.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://rau.hnqzz.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tij.gogol.net.cn

PHP:  // 手写递归函数
来源：http://rxc.mhx1999.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xxn.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nzf.tarul.cn

Java: // 手写递归
来源：http://hyz.tarul.cn


<!-- 参考信息 -->