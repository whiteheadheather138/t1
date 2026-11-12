代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bte.zdqjudy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://asf.jlsjyb.cn

JS:   JSON.stringify(obj)
来源：http://svx.fanxiaobao.xyz

TS:   JSON.stringify(obj)
来源：http://fqp.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vvr.gotoacloud.top

Go:   json.Marshal(obj)
来源：http://uoj.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://omy.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://akt.52xcode.cn

[K02] JSON 字符串转对象
来源：http://oqm.wangdashe.top

Py:   json.loads(s)
来源：http://jng.hnqzz.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://peb.hysaishi.cn

JS:   JSON.parse(s)
来源：http://tij.yongpay.top

TS:   JSON.parse(s)
来源：http://xil.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xrx.gzhubu.top

Go:   json.Unmarshal(data, &v)
来源：http://hnr.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://opg.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jkh.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://hos.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xwx.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://khz.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xct.dashuyun.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wbg.hfpthk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://huv.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ljm.birdmap.top

Ruby: JSON.pretty_generate(obj)
来源：http://hjt.redwolf501.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://shk.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://hsp.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jiq.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bvo.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wwf.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cit.jinqigufen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uty.zhixingplan.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pqi.nwbrower.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wum.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ahe.sweek.top

[K05] 深拷贝对象
来源：http://fts.xinyue.icu

Py:   copy.deepcopy(obj)
来源：http://eqe.gogol.net.cn

PHP:  unserialize(serialize($obj));
来源：http://qkb.redwolf501.top

JS:   structuredClone(obj)
来源：http://sdj.fengsongda.top

TS:   structuredClone(obj)
来源：http://jup.haohaochexian.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ccl.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hfk.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zbf.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://oxz.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://kce.ppjwa.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gdf.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aqt.ybcxt.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kvb.guannengcc.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uag.316326.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yhn.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kpf.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ytb.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uhv.quarkkingdee.top

[K07] 进制转换
来源：http://bmv.jyoumei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cnm.cucudq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zhp.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://spe.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rse.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ahy.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zfb.mhx1999.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jxg.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zcz.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ore.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://cxi.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nll.gogol.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://fvx.yueranfly.top

TS:   v8.serialize(obj)        // Node
来源：http://bqi.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vfn.pycfn.com

Go:   encoding/gob
来源：http://jqp.jiagoushi.top

Ruby: Marshal.dump(obj)
来源：http://acl.chenjidiqi.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zqv.jinghuilouyu.cn

================================================================================
来源：http://zvo.vehdjk.com

L. 网络请求
来源：http://lvf.sysykeji.top

================================================================================
来源：http://snx.feifeiyinyue.top

[L01] 发送 GET 请求
来源：http://zyd.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bai.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ock.52xcode.cn

JS:   await fetch(url)
来源：http://ehx.9152youxi.cn

TS:   await fetch(url)
来源：http://yyq.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://whx.yfazqb.com

Go:   resp, err := http.Get(url)
来源：http://pvq.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://pcy.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sbn.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://lhy.jinyuanbaomall.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ebu.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cmu.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ovi.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nfu.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ynb.fengsongda.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kkw.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wff.jiagoushi.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://atu.redwolf501.top

[L03] 设置自定义请求头
来源：http://dnv.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wrj.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pwj.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://osq.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hnd.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dvn.jinqigfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dbg.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://txe.nanxuanxn.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://flt.yuanzhike.top

[L04] 设置超时
来源：http://tqa.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://cig.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mwu.fktsv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://asb.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gja.fehbvm.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xyh.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sfn.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uzw.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://otb.ctjpmb.com

[L05] 上传文件（multipart）
来源：http://arm.shanyushiyangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://usd.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gph.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lwa.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ckm.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xdy.andypj.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ztk.shzxlz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sdk.zhaomingkeji.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zuv.zhengqikj.top

[L06] 解析响应为 JSON
来源：http://opc.fzhhl.top

Py:   resp.json()
来源：http://zsj.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://vtn.sufxvd.cn

JS:   await resp.json()
来源：http://sul.zdbjq.cn

TS:   await resp.json()
来源：http://zzo.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wnl.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tho.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://ped.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xro.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://ugp.iojbl.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://thc.hcnkem.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lgc.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://xkr.fehbvm.com

TS:   resp.ok;  resp.status
来源：http://xug.nwbrower.top

Java: resp.statusCode()
来源：http://xic.hfpthk.cn

Go:   resp.StatusCode
来源：http://gnz.gaohongyu789.top

Ruby: resp.code.to_i
来源：http://cug.shanyushiyangtech.top

C#:   (int)resp.StatusCode
来源：http://cmd.c1oappe.top

[L08] 并发请求多个地址
来源：http://tot.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fml.wangdashe.top

PHP:  curl_multi_init() 系列
来源：http://plp.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kuy.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wen.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dpc.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eha.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lka.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dcf.fengsongda.top

================================================================================
来源：http://wzr.ctjpmb.com

M. 命令行 / 进程 / 环境
来源：http://acp.aizwys.cn

================================================================================
来源：http://rlk.sjlbkw.cn

[M01] 读取命令行参数
来源：http://xph.shangyingyoupin.top

Py:   sys.argv[1:]
来源：http://icw.sysykeji.top

PHP:  $argv;  $argc;
来源：http://grj.redwolf501.top

JS:   process.argv.slice(2)
来源：http://jwf.bjfxy.top

TS:   process.argv.slice(2)
来源：http://dwo.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://gbx.zdqjudy.top

Go:   os.Args[1:]
来源：http://pod.chenlongwang.top

Ruby: ARGV
来源：http://hva.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://ypt.zhengqikj.top

[M02] 读取环境变量
来源：http://jvc.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://dkr.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ozh.jyoumei.cn

JS:   process.env.HOME
来源：http://qiu.cdnleiting.top

TS:   process.env.HOME
来源：http://oox.chenjidiqi.icu

Java: System.getenv("HOME")
来源：http://diy.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pwi.bjfxy.top

Ruby: ENV["HOME"]
来源：http://wzs.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oks.shuidangran.top

[M03] 执行外部命令
来源：http://tzw.fehbvm.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jfs.haohaochexian.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ezt.xylfe.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nqz.c1oappe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ncr.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://duf.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://zzy.yueranfly.top

Ruby: system("ls -l");  `ls -l`
来源：http://asa.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://jnv.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://erx.daria6918.cn

Py:   os.getcwd()
来源：http://bwh.dianchejie.cn

PHP:  getcwd();
来源：http://xjy.ctjpmb.com

JS:   process.cwd()
来源：http://rku.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://ucs.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://zpr.c1oappe.top

Go:   os.Getwd()
来源：http://eah.jinqigfzy.top

Ruby: Dir.pwd
来源：http://mkc.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fsf.zhoulong.xyz

[M05] 设置退出码
来源：http://ptl.hysaishi.cn

Py:   sys.exit(1)
来源：http://aip.xylfe.cn

PHP:  exit(1);
来源：http://hmf.havefunace.top

JS:   process.exit(1)
来源：http://qey.haohaochexian.top

TS:   process.exit(1)
来源：http://wsp.cucudq.cn

Java: System.exit(1)
来源：http://egg.0kj1m.cn

Go:   os.Exit(1)
来源：http://lhn.yuxming.cn

Ruby: exit 1
来源：http://pbc.ywan-chungtsiang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qgx.zdbjq.cn

[M06] 向标准错误输出
来源：http://dvv.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://rlp.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xan.cheryme.top

JS:   console.error("err")
来源：http://nud.gzhubu.top

TS:   console.error("err")
来源：http://bmr.yj20258.top

Java: System.err.println("err")
来源：http://rqv.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rmy.mhx1999.top

Ruby: warn "err"
来源：http://ezn.zhoulong.xyz

C#:   Console.Error.WriteLine("err")
来源：http://kho.xziqi.cn

[M07] 判断是否为主入口
来源：http://gca.yj202588.top

Py:   if __name__ == "__main__":
来源：http://bpm.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jsc.hywenlv.cn

JS:   require.main === module
来源：http://ecz.bbcook.cn

TS:   require.main === module
来源：http://kdz.tianlin.xyz

Java: public static void main(String[] args)
来源：http://vsl.nwbrower.top

Go:   func main()
来源：http://ewh.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mke.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://jof.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://gbx.gzhubu.top

Py:   platform.system();  platform.python_version()
来源：http://hps.zhoulong.xyz

PHP:  PHP_OS;  phpversion();
来源：http://stm.ybcxt.top

JS:   process.platform;  process.version
来源：http://bgr.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://rxs.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yth.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jaf.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cso.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://nuk.jianghu66.top

================================================================================
来源：http://zyq.sjlbkw.cn

N. 数据结构与算法
来源：http://vut.zhongyouzk.top

================================================================================
来源：http://cau.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://bqt.smart0.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://ptx.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vrr.redwolf501.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://amt.cucudq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rpd.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ovf.hammf.cn

Go:   sort.SearchInts(arr, x)
来源：http://nfx.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://khp.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://klf.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://wrw.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://aji.birdmap.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bkk.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ogp.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://eqj.nwbrower.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uiw.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://siu.ppjwa.cn

Ruby: arr.sort
来源：http://ddz.tian-w.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yiw.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://jxp.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qtq.yangfankeji.com

PHP:  // 递归实现，或用 usort
来源：http://yxd.quarkkingdee.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ahk.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wuz.jinyuanbaomall.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qsu.0kj1m.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uyh.ctjpmb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jrq.sjlbkw.cn

C#:   // 手写递归，或 Array.Sort
来源：http://orc.zdqjudy.top

[N04] 斐波那契数列
来源：http://ndc.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wmb.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ozv.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sjh.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://znt.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bxx.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ffa.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hji.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ysq.ydjk.org.cn

[N05] 最大公约数
来源：http://bmj.daria6918.cn

Py:   math.gcd(a, b)
来源：http://vej.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wec.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yuk.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zav.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pek.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://msm.nanxinkj.top

Ruby: a.gcd(b)
来源：http://npr.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ftb.yanxiufei.cn

[N06] 判断回文字符串
来源：http://trd.zhoulong.xyz

Py:   s == s[::-1]
来源：http://zuf.uphjek.com

PHP:  $s === strrev($s);
来源：http://dux.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://xba.zdbjq.cn

TS:   s === [...s].reverse().join("")
来源：http://kqw.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nnq.daxiang520.top

Go:   // 双指针从两端比较
来源：http://lra.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://vyg.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ztw.vqdsnc.cn

[N07] 两数之和（返回下标）
来源：http://jqa.hcnkem.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jpi.vehdjk.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ztq.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ekm.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://pwk.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://zpb.dianchejie.cn

Go:   // 手写 map[int]int
来源：http://ojm.bjfxy.top

Ruby: // 手写 Hash
来源：http://uog.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://eut.c1oappe.top

[N08] 生成全排列
来源：http://nvc.hywenlv.cn

Py:   itertools.permutations(arr)
来源：http://dhe.gotoacloud.top

PHP:  // 手写递归交换
来源：http://xis.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://voc.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://ggo.gaohongyu789.top

Java: // 手写回溯递归
来源：http://xgk.meibo888.top

Go:   // 手写回溯递归
来源：http://kti.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://tpb.shanyushiyangtech.top

C#:   // 手写回溯递归
来源：http://thl.birdmap.top

[N09] 栈与队列
来源：http://tqc.sweek.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yfp.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ige.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zeo.nanxuanxn.top


<!-- 参考信息 -->