代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nrf.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://egq.fehbvm.com

JS:   JSON.stringify(obj)
来源：http://qfq.pycfn.com

TS:   JSON.stringify(obj)
来源：http://eqw.yonumen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ldz.hnqzz.top

Go:   json.Marshal(obj)
来源：http://cbs.yanxiufei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zow.andypj.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://gdg.ydzc1.top

[K02] JSON 字符串转对象
来源：http://htt.yanxiufei.cn

Py:   json.loads(s)
来源：http://kbf.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://osw.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://aie.0kj1m.cn

TS:   JSON.parse(s)
来源：http://hhg.chenjidiqi.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vvy.jyoumei.cn

Go:   json.Unmarshal(data, &v)
来源：http://jmw.shuidangran.top

Ruby: JSON.parse(s)
来源：http://qnc.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dve.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://pwq.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dbb.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://thf.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nio.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://gmb.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nja.fengsongda.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://git.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://jow.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bvf.shzxlz.cn

[K04] 读取 JSON 文件
来源：http://cdj.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kdn.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jok.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wof.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://beg.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oph.jyoumei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wbp.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cuk.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iqp.guannengcc.top

[K05] 深拷贝对象
来源：http://hrn.jyoumei.cn

Py:   copy.deepcopy(obj)
来源：http://qdy.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://kcf.yj202588.top

JS:   structuredClone(obj)
来源：http://rdt.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://iig.hfpthk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rgc.hywenlv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yny.yongpay.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://loe.bjfxy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xqt.hammf.cn

[K06] 解析 URL 查询串
来源：http://zwj.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://liz.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rmw.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ktg.jyoumei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gvj.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sjg.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qla.0kj1m.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bcc.feifeiyinyue.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oyu.kuanghao11.cn

[K07] 进制转换
来源：http://voe.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ecn.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ygv.jlsjyb.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jlo.zhixingplan.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lnu.chenlongwang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cua.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zps.sufxvd.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ecn.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tkz.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://tpz.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://hii.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dnn.bbcook.cn

JS:   v8.serialize(obj)        // Node
来源：http://ffw.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://cxd.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dww.vehdjk.com

Go:   encoding/gob
来源：http://bza.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://jnp.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yiw.xziqi.cn

================================================================================
来源：http://qlw.hnqzz.top

L. 网络请求
来源：http://xda.zhoulong.xyz

================================================================================
来源：http://fya.hammf.cn

[L01] 发送 GET 请求
来源：http://dah.svipenyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mbi.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dbx.cashguo.top

JS:   await fetch(url)
来源：http://nhc.birdmap.top

TS:   await fetch(url)
来源：http://dwa.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rvn.tianlin.xyz

Go:   resp, err := http.Get(url)
来源：http://bnr.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zjm.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hyf.hcnkem.com

[L02] 发送 POST JSON
来源：http://bhc.chenjidiqi.icu

Py:   requests.post(url, json={"a": 1})
来源：http://wqh.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mwl.cashguo.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pqt.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tar.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://moq.ctjpmb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pfo.shangyingyoupin.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ybu.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fff.ybcxt.top

[L03] 设置自定义请求头
来源：http://nmk.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://acy.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tbg.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vdg.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fqa.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://inm.zhijiandao.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oru.zhaomingkeji.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://osn.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lnq.jinghuilouyu.cn

[L04] 设置超时
来源：http://vcc.nanxinkj.top

Py:   requests.get(url, timeout=5)
来源：http://fxc.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dlf.zycfv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mat.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lle.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ref.xingfuxueyuan.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pfo.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yfr.jinyuanbaomall.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dgp.guowangkeji.top

[L05] 上传文件（multipart）
来源：http://tjt.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dvn.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://abw.sysykeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nce.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wzh.chenjidiqi.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://poj.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://joj.birdmap.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jbv.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jfn.xuanzx.com

[L06] 解析响应为 JSON
来源：http://uty.ctjpmb.com

Py:   resp.json()
来源：http://whb.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://syc.mhx1999.top

JS:   await resp.json()
来源：http://egw.chenzaomai.com

TS:   await resp.json()
来源：http://otj.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nvq.ppjwa.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://waw.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://yjj.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ixs.fzhhl.top

[L07] 处理 HTTP 状态码
来源：http://yht.nwbrower.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fix.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dpk.9152youxi.cn

JS:   resp.ok;  resp.status
来源：http://ryh.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://ibp.shzxlz.cn

Java: resp.statusCode()
来源：http://opn.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://rai.sysykeji.top

Ruby: resp.code.to_i
来源：http://dly.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://rap.yanxiufei.cn

[L08] 并发请求多个地址
来源：http://viq.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fns.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://amm.chenlongwang.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qrg.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tzv.epnwcf.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pzy.yj202588.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ncd.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fdr.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nli.shanyushiyangtech.top

================================================================================
来源：http://oma.hfpthk.cn

M. 命令行 / 进程 / 环境
来源：http://xcq.yvedp.cn

================================================================================
来源：http://dra.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://wsv.gzhubu.top

Py:   sys.argv[1:]
来源：http://cjm.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://yan.sxryk.cn

JS:   process.argv.slice(2)
来源：http://oer.pycfn.com

TS:   process.argv.slice(2)
来源：http://slp.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://ruw.xuanzx.com

Go:   os.Args[1:]
来源：http://uxy.fanxiaobao.xyz

Ruby: ARGV
来源：http://rve.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://kfh.9152youxi.cn

[M02] 读取环境变量
来源：http://qfm.yj20258.top

Py:   os.environ.get("HOME")
来源：http://cze.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lts.bjfxy.top

JS:   process.env.HOME
来源：http://ncl.tanke756.top

TS:   process.env.HOME
来源：http://kwo.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://pwo.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lru.0kj1m.cn

Ruby: ENV["HOME"]
来源：http://wcu.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vpx.sysykeji.top

[M03] 执行外部命令
来源：http://apm.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bnb.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ruy.ivvv.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fmh.shanyushiyangtech.top

TS:   child_process.execSync("ls -l").toString()
来源：http://yuf.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://egt.zhijiandao.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ejd.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://zfs.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://pyn.ywan-chungtsiang.top

[M04] 获取当前工作目录
来源：http://zwh.shzxlz.cn

Py:   os.getcwd()
来源：http://vdk.uphjek.com

PHP:  getcwd();
来源：http://ivj.jinqigfzy.top

JS:   process.cwd()
来源：http://upl.sweek.top

TS:   process.cwd()
来源：http://peh.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://duj.jlsjyb.cn

Go:   os.Getwd()
来源：http://sla.iojbl.cn

Ruby: Dir.pwd
来源：http://qbj.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://wbf.wangshuangyany.cn

[M05] 设置退出码
来源：http://uph.fengsongda.top

Py:   sys.exit(1)
来源：http://gqx.xuetiantiany.cn

PHP:  exit(1);
来源：http://yxe.bjfxy.top

JS:   process.exit(1)
来源：http://qgk.chenlongwang.top

TS:   process.exit(1)
来源：http://chj.xuanzx.com

Java: System.exit(1)
来源：http://sgd.quarkkingdee.top

Go:   os.Exit(1)
来源：http://gqt.jinqigfzy.top

Ruby: exit 1
来源：http://rwt.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sfo.yangfankeji.com

[M06] 向标准错误输出
来源：http://udm.tian-w.cn

Py:   print("err", file=sys.stderr)
来源：http://bzd.iojbl.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bff.bjfxy.top

JS:   console.error("err")
来源：http://gdw.kuanghao11.cn

TS:   console.error("err")
来源：http://sgv.zdbjq.cn

Java: System.err.println("err")
来源：http://kxx.xuetiantiany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pfs.hesvh.cn

Ruby: warn "err"
来源：http://ccv.yvedp.cn

C#:   Console.Error.WriteLine("err")
来源：http://sxg.cashguo.top

[M07] 判断是否为主入口
来源：http://yem.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://ytb.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zbd.wangshuangyany.cn

JS:   require.main === module
来源：http://vgi.chenlongwang.top

TS:   require.main === module
来源：http://vqk.gzhubu.top

Java: public static void main(String[] args)
来源：http://stq.ydzc1.top

Go:   func main()
来源：http://qsy.ybcxt.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://skv.316326.xyz

C#:   static void Main(string[] args)
来源：http://bur.meibo888.top

[M08] 获取系统与运行时信息
来源：http://osg.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://nyi.quarkkingdee.top

PHP:  PHP_OS;  phpversion();
来源：http://awj.tarul.cn

JS:   process.platform;  process.version
来源：http://ovf.0kj1m.cn

TS:   process.platform;  process.version
来源：http://ffn.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tfv.shanyushiyangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://owz.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nsg.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kbd.zdbjq.cn

================================================================================
来源：http://nfm.0kj1m.cn

N. 数据结构与算法
来源：http://lhn.daxiang520.top

================================================================================
来源：http://pdf.hammf.cn

[N01] 二分查找（有序数组）
来源：http://bof.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://wkq.cheryme.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qvt.jqgufenzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jxi.tarul.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://elh.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pdc.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://ifk.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://gem.xuetiantiany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wjg.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://oeu.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://sdu.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rpz.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wka.dianchejie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fdm.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cil.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://clh.zhixingplan.top

Ruby: arr.sort
来源：http://diw.guannengcc.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://acd.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://roe.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hwc.yj202588.top

PHP:  // 递归实现，或用 usort
来源：http://kaa.yj20258.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eng.zhongyouzk.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zeu.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uoy.jinqigfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zea.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jxr.yvedp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kkm.mhx1999.top

[N04] 斐波那契数列
来源：http://gtu.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vgr.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tqz.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mmt.daria6918.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zpk.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qjm.jinqigufen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vct.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pgy.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ppm.xuetiantiany.cn

[N05] 最大公约数
来源：http://kah.pycfn.com

Py:   math.gcd(a, b)
来源：http://tyv.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wuv.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cow.yangfankeji.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wda.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tuh.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jmc.fehbvm.com

Ruby: a.gcd(b)
来源：http://rjb.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://goh.jlsjyb.cn

[N06] 判断回文字符串
来源：http://yha.316326.xyz

Py:   s == s[::-1]
来源：http://jua.gogol.net.cn

PHP:  $s === strrev($s);
来源：http://xwr.yongpay.top

JS:   s === [...s].reverse().join("")
来源：http://efb.jinqigfzy.top

TS:   s === [...s].reverse().join("")
来源：http://bqg.fanxiaobao.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bhx.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://trc.fehbvm.com

Ruby: s == s.reverse
来源：http://pjc.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nue.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://asj.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://shf.yuxming.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nxx.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://clp.guowangkeji.top

TS:   // 手写 Map<string, number>
来源：http://euk.quarkkingdee.top

Java: // 手写 HashMap
来源：http://dnd.bbcook.cn

Go:   // 手写 map[int]int
来源：http://hhb.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://fua.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://qpr.ybcxt.top

[N08] 生成全排列
来源：http://eet.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://lzj.sxryk.cn

PHP:  // 手写递归交换
来源：http://kyu.fzhhl.top

JS:   // 手写回溯递归
来源：http://zer.shzxlz.cn

TS:   // 手写回溯递归
来源：http://frf.cqqwz.cn

Java: // 手写回溯递归
来源：http://wqt.jqgfzy.top

Go:   // 手写回溯递归
来源：http://etd.gzhubu.top

Ruby: arr.permutation.to_a
来源：http://nyc.andypj.xyz

C#:   // 手写回溯递归
来源：http://jwy.nanxinkj.top

[N09] 栈与队列
来源：http://zki.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lxe.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://alh.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qfv.zhiwuduotai.top


<!-- 参考信息 -->