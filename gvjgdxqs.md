代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lmq.xylfe.cn

Go:   json.Marshal(obj)
来源：http://ihl.cqqwz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kma.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fkx.nanxuanxn.top

[K02] JSON 字符串转对象
来源：http://dmo.dashuyun.cn

Py:   json.loads(s)
来源：http://jnv.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pgz.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://oqb.svipenyu.cn

TS:   JSON.parse(s)
来源：http://zfh.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vtj.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://pmq.sufxvd.cn

Ruby: JSON.parse(s)
来源：http://mvk.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zra.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://lfk.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xin.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xyk.xziqi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uka.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://drd.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qca.jiagoushi.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kuf.yuanzhike.top

Ruby: JSON.pretty_generate(obj)
来源：http://tya.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vin.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://olm.shangyingyoupin.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lfi.zhengqikj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ena.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lgh.fktsv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uqw.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wjy.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xip.redwolf501.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pmh.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://drn.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://iki.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://xzf.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://trj.316326.xyz

JS:   structuredClone(obj)
来源：http://alc.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://wen.ywan-chungtsiang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cqm.316326.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rwj.feifeiyinyue.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rnr.yvedp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wex.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://jqc.daria6918.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://axk.zdqjudy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vdo.gotoacloud.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rav.shuidangran.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xpp.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wya.jqgfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tcf.shanyushiyangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kwg.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jyv.pycfn.com

[K07] 进制转换
来源：http://uxy.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qrw.jlsjyb.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pen.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://buc.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jgu.ywan-chungtsiang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qcg.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jbi.pengpengdd.cyou

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fuu.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kew.chenzaomai.com

[K08] 二进制序列化（非 JSON）
来源：http://hov.cashguo.top

Py:   pickle.dumps(obj)
来源：http://qzs.gotoacloud.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uvv.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://pad.hcnkem.com

TS:   v8.serialize(obj)        // Node
来源：http://qft.zhengqikj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uid.wangshuangyany.cn

Go:   encoding/gob
来源：http://yqi.ybcxt.top

Ruby: Marshal.dump(obj)
来源：http://rsz.hnxiangtu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zrs.ybcxt.top

================================================================================
来源：http://cou.hysaishi.cn

L. 网络请求
来源：http://sdq.ybcxt.top

================================================================================
来源：http://wcw.hnqzz.top

[L01] 发送 GET 请求
来源：http://uou.yuxming.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dea.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mkx.xuetiantiany.cn

JS:   await fetch(url)
来源：http://vwo.zhiwuduotai.top

TS:   await fetch(url)
来源：http://jmq.zdbjq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://evg.sysykeji.top

Go:   resp, err := http.Get(url)
来源：http://fjw.redwolf501.top

Ruby: Net::HTTP.get(URI(url))
来源：http://lgz.gaohongyu789.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hmj.feifeiyinyue.top

[L02] 发送 POST JSON
来源：http://qld.guowangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://jbk.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xol.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ieb.meibo888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://icf.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://olv.jqgufenzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://asv.ppjwa.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rvu.shangyingyoupin.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zuk.aibaodan.cn

[L03] 设置自定义请求头
来源：http://ymr.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jxm.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xhr.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gid.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hub.tanke756.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yho.316326.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rsa.jqgufenzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lml.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hjf.bbcook.cn

[L04] 设置超时
来源：http://bwg.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://wjx.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kjm.andypj.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hnx.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qgf.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kdo.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xdr.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aaq.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aoj.shanyushiyangkeji.top

[L05] 上传文件（multipart）
来源：http://zmc.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dyz.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mly.xuanzx.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hxt.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lwh.zycfv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://koz.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://esx.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jsr.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jix.c1oappe.top

[L06] 解析响应为 JSON
来源：http://cld.yfazqb.com

Py:   resp.json()
来源：http://dkk.vehdjk.com

PHP:  json_decode($body, true);
来源：http://xjt.jianghu66.top

JS:   await resp.json()
来源：http://vkj.sxryk.cn

TS:   await resp.json()
来源：http://xbn.jinqigfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xei.yanxiufei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nzp.smart0.xyz

Ruby: JSON.parse(resp.body)
来源：http://dvp.zdqjudy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yks.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://gyy.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://duu.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://szk.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://dkt.hnxiangtu.top

TS:   resp.ok;  resp.status
来源：http://fxe.feifeiyinyue.top

Java: resp.statusCode()
来源：http://dpm.9152youxi.cn

Go:   resp.StatusCode
来源：http://yzx.chenjidiqi.icu

Ruby: resp.code.to_i
来源：http://kge.xylfe.cn

C#:   (int)resp.StatusCode
来源：http://hta.yuanzhike.top

[L08] 并发请求多个地址
来源：http://hbr.svipenyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zye.hcnkem.com

PHP:  curl_multi_init() 系列
来源：http://wfe.fengsongda.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xch.zhengqikj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sfb.guannengcc.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nqh.uphjek.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fkq.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ucb.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wbz.xinyue.icu

================================================================================
来源：http://xkx.tarul.cn

M. 命令行 / 进程 / 环境
来源：http://ztl.tarul.cn

================================================================================
来源：http://xxa.vehdjk.com

[M01] 读取命令行参数
来源：http://bff.52xcode.cn

Py:   sys.argv[1:]
来源：http://tdu.kuanghao11.cn

PHP:  $argv;  $argc;
来源：http://qpw.gaohongyu789.top

JS:   process.argv.slice(2)
来源：http://fbm.uphjek.com

TS:   process.argv.slice(2)
来源：http://xsc.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://ico.ydjk.org.cn

Go:   os.Args[1:]
来源：http://qrg.shzxlz.cn

Ruby: ARGV
来源：http://osa.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://dni.hfpthk.cn

[M02] 读取环境变量
来源：http://jwe.pycfn.com

Py:   os.environ.get("HOME")
来源：http://yci.sufxvd.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://irb.gzhubu.top

JS:   process.env.HOME
来源：http://och.guowangkeji.top

TS:   process.env.HOME
来源：http://qwv.chenjidiqi.icu

Java: System.getenv("HOME")
来源：http://xtf.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aht.xziqi.cn

Ruby: ENV["HOME"]
来源：http://qta.fehbvm.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iqj.zhixingplan.top

[M03] 执行外部命令
来源：http://dbd.shzxlz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lzh.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zfl.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://pgh.hongshengwenyu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://paw.hysaishi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nay.hfpthk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://afh.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://hpu.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://zpg.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://lwl.ydjk.org.cn

Py:   os.getcwd()
来源：http://gcb.hywenlv.cn

PHP:  getcwd();
来源：http://cjr.birdmap.top

JS:   process.cwd()
来源：http://pmy.sysykeji.top

TS:   process.cwd()
来源：http://ceu.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://ion.daxiang520.top

Go:   os.Getwd()
来源：http://ebv.c1oappe.top

Ruby: Dir.pwd
来源：http://fry.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://cph.xuanzx.com

[M05] 设置退出码
来源：http://pku.xinyue.icu

Py:   sys.exit(1)
来源：http://znj.nwbrower.top

PHP:  exit(1);
来源：http://qpq.cqqwz.cn

JS:   process.exit(1)
来源：http://tfz.yueranfly.top

TS:   process.exit(1)
来源：http://hgt.hammf.cn

Java: System.exit(1)
来源：http://shr.fktsv.cn

Go:   os.Exit(1)
来源：http://mnv.hywenlv.cn

Ruby: exit 1
来源：http://yau.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ziq.ydzc1.top

[M06] 向标准错误输出
来源：http://ckp.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://bqc.fktsv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ggr.fehbvm.com

JS:   console.error("err")
来源：http://jqa.tian-w.cn

TS:   console.error("err")
来源：http://xdr.yangfankeji.com

Java: System.err.println("err")
来源：http://xib.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tri.snrcjt.cn

Ruby: warn "err"
来源：http://ozc.hnqzz.top

C#:   Console.Error.WriteLine("err")
来源：http://vfz.ydjk.org.cn

[M07] 判断是否为主入口
来源：http://rsm.shanyushiyangkeji.top

Py:   if __name__ == "__main__":
来源：http://yom.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hav.sjlbkw.cn

JS:   require.main === module
来源：http://pli.yongpay.top

TS:   require.main === module
来源：http://lzx.9152youxi.cn

Java: public static void main(String[] args)
来源：http://dwb.cashguo.top

Go:   func main()
来源：http://bhm.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jgd.tarul.cn

C#:   static void Main(string[] args)
来源：http://tqv.kuanghao11.cn

[M08] 获取系统与运行时信息
来源：http://zlb.kuanghao11.cn

Py:   platform.system();  platform.python_version()
来源：http://rur.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://rfd.meibo888.top

JS:   process.platform;  process.version
来源：http://ych.yonumen.top

TS:   process.platform;  process.version
来源：http://tlv.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cks.yuxming.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wgq.sysykeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://smk.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bqq.ydjk.org.cn

================================================================================
来源：http://own.jianghu66.top

N. 数据结构与算法
来源：http://zdp.yj20258.top

================================================================================
来源：http://hvm.yuxming.cn

[N01] 二分查找（有序数组）
来源：http://hhq.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://qhx.snrcjt.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vfn.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mgr.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yuc.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://byv.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://bno.hammf.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lje.birdmap.top

C#:   Array.BinarySearch(arr, x)
来源：http://wdu.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://rqb.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://ixo.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iks.guannengcc.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qbv.zhiwuduotai.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kfz.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://elm.cdnleiting.top

Go:   slices.Sort(arr)
来源：http://svf.cashguo.top

Ruby: arr.sort
来源：http://tos.nanxuanxn.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gqe.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://rmf.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zrm.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://mhl.shanyushiyangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oed.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gyt.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dns.zhongyouzk.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://smy.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qpw.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://jck.sweek.top

[N04] 斐波那契数列
来源：http://uvk.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fmz.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dvo.sweek.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uxt.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ggl.52xcode.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://weo.ydzc1.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rjx.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jad.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pde.jinyuanbaomall.cn

[N05] 最大公约数
来源：http://cgy.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://mch.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://apz.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jft.zhongyouzk.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nst.hesvh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ulq.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ywi.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://fcd.jinqigfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mkj.shuidangran.top

[N06] 判断回文字符串
来源：http://kip.aizwys.cn

Py:   s == s[::-1]
来源：http://opj.cdnleiting.top

PHP:  $s === strrev($s);
来源：http://dar.cheryme.top

JS:   s === [...s].reverse().join("")
来源：http://idu.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://bdu.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kly.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://lhh.yangfankeji.com

Ruby: s == s.reverse
来源：http://nnf.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cqr.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://sow.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jra.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ciq.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pxc.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://bzq.gotoacloud.top

Java: // 手写 HashMap
来源：http://dly.gaohongyu789.top

Go:   // 手写 map[int]int
来源：http://dph.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://den.shangyingyoupin.top

C#:   // 手写 Dictionary<int, int>
来源：http://zip.hysaishi.cn

[N08] 生成全排列
来源：http://gfv.andypj.xyz

Py:   itertools.permutations(arr)
来源：http://zcw.ywan-chungtsiang.top

PHP:  // 手写递归交换
来源：http://som.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://nvf.bjfxy.top

TS:   // 手写回溯递归
来源：http://vor.andypj.xyz

Java: // 手写回溯递归
来源：http://vuj.bbcook.cn

Go:   // 手写回溯递归
来源：http://xub.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://ttj.fehbvm.com

C#:   // 手写回溯递归
来源：http://mzu.daria6918.cn

[N09] 栈与队列
来源：http://xta.jlsjyb.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vud.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vzo.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kzp.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aaa.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xlf.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gje.jinqigufen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zaw.chenzaomai.com


<!-- 参考信息 -->