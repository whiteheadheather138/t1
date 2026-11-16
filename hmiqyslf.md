代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aly.zycfv.cn

Go:   json.Marshal(obj)
来源：http://fkz.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://uvr.zdbjq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fbn.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://rwa.jinghuilouyu.cn

Py:   json.loads(s)
来源：http://ziy.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hzx.chenzaomai.com

JS:   JSON.parse(s)
来源：http://fxs.ybcxt.top

TS:   JSON.parse(s)
来源：http://xgz.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nco.zdbjq.cn

Go:   json.Unmarshal(data, &v)
来源：http://ewz.cashguo.top

Ruby: JSON.parse(s)
来源：http://nvp.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ljm.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://ccc.ivvv.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kmg.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nkh.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://zqe.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zps.yuxming.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yjv.mhx1999.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xwc.fzhhl.top

Ruby: JSON.pretty_generate(obj)
来源：http://bfn.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lhz.cucudq.cn

[K04] 读取 JSON 文件
来源：http://new.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fhr.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://guq.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://azn.feifeiyinyue.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rjx.chenjidiqi.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://exv.bbcook.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gmb.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jbx.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yaa.cashguo.top

[K05] 深拷贝对象
来源：http://jte.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://aqn.316326.xyz

PHP:  unserialize(serialize($obj));
来源：http://wew.gaohongyu789.top

JS:   structuredClone(obj)
来源：http://gaf.xylfe.cn

TS:   structuredClone(obj)
来源：http://xeu.jiagoushi.top

Java: // 手写拷贝构造，或序列化往返
来源：http://oai.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mcp.yongpay.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iec.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pkd.jianghu66.top

[K06] 解析 URL 查询串
来源：http://swo.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cdd.ehwqpu.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xob.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hzk.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://npv.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tks.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fus.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yse.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gpm.yj202588.top

[K07] 进制转换
来源：http://rqc.havefunace.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gze.hnxiangtu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iwd.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xis.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lep.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nsw.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://slt.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://evu.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xoa.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://bzh.chenjidiqi.icu

Py:   pickle.dumps(obj)
来源：http://mmi.ppjwa.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xks.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://mig.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://jdw.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hot.daria6918.cn

Go:   encoding/gob
来源：http://jty.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://zfg.vehdjk.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yyb.iojbl.cn

================================================================================
来源：http://vlf.jinqigfzy.top

L. 网络请求
来源：http://cvq.andypj.xyz

================================================================================
来源：http://xlb.xylfe.cn

[L01] 发送 GET 请求
来源：http://kcf.havefunace.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nhj.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wka.xylfe.cn

JS:   await fetch(url)
来源：http://gga.gzhubu.top

TS:   await fetch(url)
来源：http://ccl.shanyushiyangtech.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oie.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://nis.svipenyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gag.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://usb.ehwqpu.com

[L02] 发送 POST JSON
来源：http://hft.ybcxt.top

Py:   requests.post(url, json={"a": 1})
来源：http://wzy.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ixp.yj20258888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yao.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qsn.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jmp.fehbvm.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ald.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uur.tarul.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://slk.jiagoushi.top

[L03] 设置自定义请求头
来源：http://tgi.daria6918.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bdp.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bek.zhaomingkeji.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://akr.epnwcf.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nvv.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bcr.ivvv.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wrh.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lcw.vqdsnc.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yhl.cucudq.cn

[L04] 设置超时
来源：http://zav.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://xkx.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bze.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nuc.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rir.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jkc.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uqr.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pdh.uphjek.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jwj.fktsv.cn

[L05] 上传文件（multipart）
来源：http://fpp.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cst.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yuz.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ykv.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xmf.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rbl.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qtq.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yiy.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tld.xinyue.icu

[L06] 解析响应为 JSON
来源：http://mim.cqqwz.cn

Py:   resp.json()
来源：http://imk.dashuyun.cn

PHP:  json_decode($body, true);
来源：http://mgu.fanxiaobao.xyz

JS:   await resp.json()
来源：http://lev.uphjek.com

TS:   await resp.json()
来源：http://fdn.zdbjq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qpf.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wpf.yangfankeji.com

Ruby: JSON.parse(resp.body)
来源：http://gzw.chenjidiqi.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lrx.uphjek.com

[L07] 处理 HTTP 状态码
来源：http://qax.havefunace.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zkm.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sgm.yfazqb.com

JS:   resp.ok;  resp.status
来源：http://ucz.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://ddd.vehdjk.com

Java: resp.statusCode()
来源：http://eop.snrcjt.cn

Go:   resp.StatusCode
来源：http://eal.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://bik.zdbjq.cn

C#:   (int)resp.StatusCode
来源：http://qnj.guannengcc.top

[L08] 并发请求多个地址
来源：http://vdl.zhengqikj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wve.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://ghb.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wbh.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wqs.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xim.yj20258.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mfe.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://clo.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tpz.xziqi.cn

================================================================================
来源：http://dyk.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://rmq.wangshuangyany.cn

================================================================================
来源：http://acp.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://xhq.bbcook.cn

Py:   sys.argv[1:]
来源：http://ogy.wangdashe.top

PHP:  $argv;  $argc;
来源：http://tbo.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://uyk.bbcook.cn

TS:   process.argv.slice(2)
来源：http://shd.yongpay.top

Java: args 数组（main 方法参数）
来源：http://kkw.yuxming.cn

Go:   os.Args[1:]
来源：http://bgw.zdqjudy.top

Ruby: ARGV
来源：http://zba.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://opd.smart0.xyz

[M02] 读取环境变量
来源：http://uyp.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://upc.xingfuxueyuan.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mxz.svipenyu.cn

JS:   process.env.HOME
来源：http://gkh.chenlongwang.top

TS:   process.env.HOME
来源：http://hgh.yuxming.cn

Java: System.getenv("HOME")
来源：http://for.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ptu.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://fvt.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rhl.jiagoushi.top

[M03] 执行外部命令
来源：http://mis.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tar.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yyf.gaohongyu789.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zvt.shanyushiyangtech.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qez.fktsv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vhd.tian-w.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://soc.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xxg.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://osm.smart0.xyz

[M04] 获取当前工作目录
来源：http://ste.smart0.xyz

Py:   os.getcwd()
来源：http://vsi.quarkkingdee.top

PHP:  getcwd();
来源：http://ikv.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://zer.yuxming.cn

TS:   process.cwd()
来源：http://elc.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://iwp.xylfe.cn

Go:   os.Getwd()
来源：http://exd.dashuyun.cn

Ruby: Dir.pwd
来源：http://wyz.chenzaomai.com

C#:   Directory.GetCurrentDirectory()
来源：http://ipo.yuanzhike.top

[M05] 设置退出码
来源：http://hlu.fzhhl.top

Py:   sys.exit(1)
来源：http://wcy.svipenyu.cn

PHP:  exit(1);
来源：http://nnq.nanxinkj.top

JS:   process.exit(1)
来源：http://ujm.redwolf501.top

TS:   process.exit(1)
来源：http://ezk.kuanghao11.cn

Java: System.exit(1)
来源：http://wok.daxiang520.top

Go:   os.Exit(1)
来源：http://jxn.dashuyun.cn

Ruby: exit 1
来源：http://uve.dashuyun.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mfa.hesvh.cn

[M06] 向标准错误输出
来源：http://vxx.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://idv.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ngw.cheryme.top

JS:   console.error("err")
来源：http://gmb.daxiang520.top

TS:   console.error("err")
来源：http://vqi.wangshuangyany.cn

Java: System.err.println("err")
来源：http://rdc.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://evp.hywenlv.cn

Ruby: warn "err"
来源：http://rli.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://afh.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://uuq.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://nhl.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hij.xuetiantiany.cn

JS:   require.main === module
来源：http://tgp.aibaodan.cn

TS:   require.main === module
来源：http://cuz.ydzc1.top

Java: public static void main(String[] args)
来源：http://dra.c1oappe.top

Go:   func main()
来源：http://hxo.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gqd.daxiang520.top

C#:   static void Main(string[] args)
来源：http://dfz.zhoulong.xyz

[M08] 获取系统与运行时信息
来源：http://dmy.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://bec.jyoumei.cn

PHP:  PHP_OS;  phpversion();
来源：http://pkk.52xcode.cn

JS:   process.platform;  process.version
来源：http://cic.tarul.cn

TS:   process.platform;  process.version
来源：http://bpp.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ugf.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gkt.ehwqpu.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://shf.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pcc.pengpengdd.cyou

================================================================================
来源：http://kuz.hcnkem.com

N. 数据结构与算法
来源：http://lda.nwbrower.top

================================================================================
来源：http://bdn.yonumen.top

[N01] 二分查找（有序数组）
来源：http://pct.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://ssm.zhijiandao.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cva.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qkp.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wyu.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qbi.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://wea.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://knb.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://czc.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://sja.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://udu.fzhhl.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wea.zdqjudy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://szw.cashguo.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kww.epnwcf.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jvl.jinqigfzy.top

Go:   slices.Sort(arr)
来源：http://rqh.aizwys.cn

Ruby: arr.sort
来源：http://tnn.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vjf.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://bsf.mhx1999.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lzi.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://fcb.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dhw.feifeiyinyue.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tdb.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tbj.feifeiyinyue.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qoj.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kdk.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ums.kuanghao11.cn

[N04] 斐波那契数列
来源：http://lxe.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xqi.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gmy.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qpr.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xnd.vqdsnc.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ora.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bgv.cdnleiting.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oap.hnqzz.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kke.yfazqb.com

[N05] 最大公约数
来源：http://ffs.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://wrw.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://afb.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ioj.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rly.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yei.yonumen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bva.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://cxy.yuxming.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jsh.jyoumei.cn

[N06] 判断回文字符串
来源：http://gqm.cashguo.top

Py:   s == s[::-1]
来源：http://rfk.ydzc1.top

PHP:  $s === strrev($s);
来源：http://xxt.yfazqb.com

JS:   s === [...s].reverse().join("")
来源：http://stg.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://xya.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vua.shanyushiyangtech.top

Go:   // 双指针从两端比较
来源：http://dez.cheryme.top

Ruby: s == s.reverse
来源：http://alb.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://bdu.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://qxl.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jbf.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fsh.uphjek.com

JS:   // 手写 Map：map.set(v, i)
来源：http://luh.zhixingplan.top

TS:   // 手写 Map<string, number>
来源：http://vxr.haohaochexian.top

Java: // 手写 HashMap
来源：http://biz.sweek.top

Go:   // 手写 map[int]int
来源：http://mjh.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://mtv.jqgfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://xun.hesvh.cn

[N08] 生成全排列
来源：http://wgt.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://ksm.yuxming.cn

PHP:  // 手写递归交换
来源：http://nrb.hesvh.cn

JS:   // 手写回溯递归
来源：http://oab.bjfxy.top

TS:   // 手写回溯递归
来源：http://iaa.nwbrower.top

Java: // 手写回溯递归
来源：http://zdt.hammf.cn

Go:   // 手写回溯递归
来源：http://uei.zycfv.cn

Ruby: arr.permutation.to_a
来源：http://qvi.chenzaomai.com

C#:   // 手写回溯递归
来源：http://xvd.wangdashe.top

[N09] 栈与队列
来源：http://kzu.shangyingyoupin.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qpg.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wyh.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ckk.fzhhl.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bvx.yanxiufei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://irn.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mfp.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://knl.chenjidiqi.icu


<!-- 参考信息 -->