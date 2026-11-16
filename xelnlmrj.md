代发 wailian999

TS:   JSON.parse(s)
来源：http://bde.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://umq.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://yqy.hesvh.cn

Ruby: JSON.parse(s)
来源：http://brt.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ezx.zhengqikj.top

[K03] JSON 美化输出（带缩进）
来源：http://dhi.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ebh.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ngb.zhoulong.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://ofp.jqgfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rri.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ulh.xuanzx.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wmh.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pgh.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wbx.havefunace.top

[K04] 读取 JSON 文件
来源：http://mrk.fengsongda.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ujn.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://svq.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jbo.yvedp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qip.ppjwa.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vuf.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mib.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uyj.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kqc.52xcode.cn

[K05] 深拷贝对象
来源：http://aga.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://gwn.ivvv.top

PHP:  unserialize(serialize($obj));
来源：http://zzk.c1oappe.top

JS:   structuredClone(obj)
来源：http://bja.ydzc1.top

TS:   structuredClone(obj)
来源：http://wcm.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://etr.vehdjk.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eon.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://urk.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://eyx.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://itx.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xsg.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rxh.jiagoushi.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zbx.zhijiandao.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dxd.zdbjq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lod.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ral.wangshuangyany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vtc.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://icm.hfpthk.cn

[K07] 进制转换
来源：http://lfl.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tkt.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eww.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iqf.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vrk.hnxiangtu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dgi.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hkq.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ghb.sxryk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tgo.hesvh.cn

[K08] 二进制序列化（非 JSON）
来源：http://rqq.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://gvc.jianghu66.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qbe.pengpengdd.cyou

JS:   v8.serialize(obj)        // Node
来源：http://uis.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://fzo.yueranfly.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nfp.yvedp.cn

Go:   encoding/gob
来源：http://fav.yj20258888.top

Ruby: Marshal.dump(obj)
来源：http://vid.yanxiufei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bys.nwbrower.top

================================================================================
来源：http://pba.zdbjq.cn

L. 网络请求
来源：http://fix.xuanzx.com

================================================================================
来源：http://ajf.yj20258.top

[L01] 发送 GET 请求
来源：http://ghl.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ruz.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uxl.andypj.xyz

JS:   await fetch(url)
来源：http://jfs.meibo888.top

TS:   await fetch(url)
来源：http://fsb.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mfk.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://vqs.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wbk.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vob.ydzc1.top

[L02] 发送 POST JSON
来源：http://rku.hnqzz.top

Py:   requests.post(url, json={"a": 1})
来源：http://euw.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://euq.haohaochexian.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ifq.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kse.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://klt.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yqc.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bab.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hju.yuanzhike.top

[L03] 设置自定义请求头
来源：http://vqz.zdqjudy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xiu.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vqn.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ize.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ear.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gcw.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zgz.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lsn.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kbe.cucudq.cn

[L04] 设置超时
来源：http://sxz.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://rcg.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sek.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lfp.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hqz.bbcook.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oom.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dvd.wangshuangyany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ocd.52xcode.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wgr.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://lcv.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kzj.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kht.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cda.xuetiantiany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aed.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://osj.vqdsnc.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vvf.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jxe.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qcw.gogol.net.cn

[L06] 解析响应为 JSON
来源：http://vnx.cdnleiting.top

Py:   resp.json()
来源：http://fyx.52xcode.cn

PHP:  json_decode($body, true);
来源：http://dvc.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://tkc.hcnkem.com

TS:   await resp.json()
来源：http://oab.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xtb.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ghu.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://ghr.bjfxy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iet.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://uvp.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://asp.svipenyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dhx.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://wis.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://dvs.yvedp.cn

Java: resp.statusCode()
来源：http://cgm.9152youxi.cn

Go:   resp.StatusCode
来源：http://xya.9152youxi.cn

Ruby: resp.code.to_i
来源：http://soe.yuxming.cn

C#:   (int)resp.StatusCode
来源：http://zql.tarul.cn

[L08] 并发请求多个地址
来源：http://pep.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wea.havefunace.top

PHP:  curl_multi_init() 系列
来源：http://cbe.nanxinkj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jua.fanxiaobao.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hgh.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zkm.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mlt.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kga.gaohongyu789.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lht.jinghuilouyu.cn

================================================================================
来源：http://ezv.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://yip.hnqzz.top

================================================================================
来源：http://xfu.yueranfly.top

[M01] 读取命令行参数
来源：http://eat.xingfuxueyuan.xyz

Py:   sys.argv[1:]
来源：http://btk.bbcook.cn

PHP:  $argv;  $argc;
来源：http://zuy.jinqigufen.top

JS:   process.argv.slice(2)
来源：http://ybn.cashguo.top

TS:   process.argv.slice(2)
来源：http://znp.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://hjw.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://tpy.jinqigfzy.top

Ruby: ARGV
来源：http://uhd.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://mot.yj202588.top

[M02] 读取环境变量
来源：http://mrh.hnqzz.top

Py:   os.environ.get("HOME")
来源：http://krc.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wji.fktsv.cn

JS:   process.env.HOME
来源：http://csr.nanxinkj.top

TS:   process.env.HOME
来源：http://ybi.hysaishi.cn

Java: System.getenv("HOME")
来源：http://lmn.kuanghao11.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://omu.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://ftj.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ysv.gogol.net.cn

[M03] 执行外部命令
来源：http://jsn.ctjpmb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xrg.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://anw.ctjpmb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://noc.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nyr.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://puq.redwolf501.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zis.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hga.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://sgq.dianchejie.cn

[M04] 获取当前工作目录
来源：http://znl.ppjwa.cn

Py:   os.getcwd()
来源：http://jvw.chenzaomai.com

PHP:  getcwd();
来源：http://dsf.gogol.net.cn

JS:   process.cwd()
来源：http://stl.zhiwuduotai.top

TS:   process.cwd()
来源：http://lva.jinqigfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://wbe.aibaodan.cn

Go:   os.Getwd()
来源：http://xgf.sufxvd.cn

Ruby: Dir.pwd
来源：http://egn.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://add.hfpthk.cn

[M05] 设置退出码
来源：http://jek.cqqwz.cn

Py:   sys.exit(1)
来源：http://vaq.xziqi.cn

PHP:  exit(1);
来源：http://gju.xuetiantiany.cn

JS:   process.exit(1)
来源：http://hok.nanxinkj.top

TS:   process.exit(1)
来源：http://utg.316326.xyz

Java: System.exit(1)
来源：http://xra.jinqigufen.top

Go:   os.Exit(1)
来源：http://cqh.gzhubu.top

Ruby: exit 1
来源：http://jlr.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blz.jiagoushi.top

[M06] 向标准错误输出
来源：http://ocm.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://eai.ppjwa.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qvf.ivvv.top

JS:   console.error("err")
来源：http://kog.fengsongda.top

TS:   console.error("err")
来源：http://wjx.hammf.cn

Java: System.err.println("err")
来源：http://bhk.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kez.zycfv.cn

Ruby: warn "err"
来源：http://ifn.uphjek.com

C#:   Console.Error.WriteLine("err")
来源：http://ccu.tianlin.xyz

[M07] 判断是否为主入口
来源：http://cqx.mhx1999.top

Py:   if __name__ == "__main__":
来源：http://ffq.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vjn.chenzaomai.com

JS:   require.main === module
来源：http://dtg.havefunace.top

TS:   require.main === module
来源：http://qun.9152youxi.cn

Java: public static void main(String[] args)
来源：http://qfj.haohaochexian.top

Go:   func main()
来源：http://pqv.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qnf.jinqigufen.top

C#:   static void Main(string[] args)
来源：http://zhp.316326.xyz

[M08] 获取系统与运行时信息
来源：http://qhw.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://ygn.nwbrower.top

PHP:  PHP_OS;  phpversion();
来源：http://gwr.guowangkeji.top

JS:   process.platform;  process.version
来源：http://khb.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://iub.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zgq.fktsv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qxu.jqgufenzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ibt.yj20258888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lwx.svipenyu.cn

================================================================================
来源：http://lxs.xylfe.cn

N. 数据结构与算法
来源：http://xgk.sweek.top

================================================================================
来源：http://kjw.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://thn.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://bxy.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kyp.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nyn.redwolf501.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gym.hesvh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hwp.xuanzx.com

Go:   sort.SearchInts(arr, x)
来源：http://ndr.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tkb.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://qza.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://uty.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://tun.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kmu.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dqe.bbcook.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pkr.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hhb.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://eep.aizwys.cn

Ruby: arr.sort
来源：http://lxy.sweek.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://sgy.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://ppf.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yku.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://qhu.bbcook.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uvo.ppjwa.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uxi.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tav.gaohongyu789.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rns.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://efk.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://yha.fktsv.cn

[N04] 斐波那契数列
来源：http://vwk.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eph.epnwcf.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://srb.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oax.cqqwz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xgb.smart0.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kgo.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eui.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fht.zhixingplan.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hda.yfazqb.com

[N05] 最大公约数
来源：http://lqp.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://jdz.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eht.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qju.sxryk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rty.hnxiangtu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dlo.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fvj.gogol.net.cn

Ruby: a.gcd(b)
来源：http://bvy.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xjs.tanke756.top

[N06] 判断回文字符串
来源：http://kqx.jiagoushi.top

Py:   s == s[::-1]
来源：http://vus.kuanghao11.cn

PHP:  $s === strrev($s);
来源：http://eem.ctjpmb.com

JS:   s === [...s].reverse().join("")
来源：http://qlq.feifeiyinyue.top

TS:   s === [...s].reverse().join("")
来源：http://twu.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gus.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://jsh.hammf.cn

Ruby: s == s.reverse
来源：http://ehv.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fwt.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://czm.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lei.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://abh.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://feq.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://hzk.fehbvm.com

Java: // 手写 HashMap
来源：http://scn.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://vwo.fzhhl.top

Ruby: // 手写 Hash
来源：http://wdx.yj20258.top

C#:   // 手写 Dictionary<int, int>
来源：http://szn.xinyue.icu

[N08] 生成全排列
来源：http://odq.haohaochexian.top

Py:   itertools.permutations(arr)
来源：http://jwb.jqgfzy.top

PHP:  // 手写递归交换
来源：http://pay.aibaodan.cn

JS:   // 手写回溯递归
来源：http://fzl.shangyingyoupin.top

TS:   // 手写回溯递归
来源：http://vnm.chenjidiqi.icu

Java: // 手写回溯递归
来源：http://lkr.meibo888.top

Go:   // 手写回溯递归
来源：http://vwz.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://gaa.jinqigufen.top

C#:   // 手写回溯递归
来源：http://xhf.jinqigfzy.top

[N09] 栈与队列
来源：http://vco.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ubd.yanxiufei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://exy.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vsz.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://quc.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lcz.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oad.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hvm.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lvg.gotoacloud.top

[N10] 链表节点定义
来源：http://yfe.zdbjq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yht.fengsongda.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ulj.tianlin.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kcl.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pep.ydjk.org.cn

Java: class Node { int v; Node next; }
来源：http://uwf.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://rfz.xylfe.cn


<!-- 参考信息 -->