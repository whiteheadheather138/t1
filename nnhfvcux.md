代发 wailian999

================================================================================
来源：http://pzm.nanxuanxn.top

K. JSON 与序列化
来源：http://rop.guowangkeji.top

================================================================================
来源：http://mgj.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://vyv.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tks.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ghd.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://wwk.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://klf.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fav.birdmap.top

Go:   json.Marshal(obj)
来源：http://ftv.ctjpmb.com

Ruby: obj.to_json                                     // require "json"
来源：http://wjl.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vkp.xziqi.cn

[K02] JSON 字符串转对象
来源：http://ysr.jinghuilouyu.cn

Py:   json.loads(s)
来源：http://pvi.hnqzz.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bbb.daxiang520.top

JS:   JSON.parse(s)
来源：http://egt.fanxiaobao.xyz

TS:   JSON.parse(s)
来源：http://tez.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tey.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://khk.smart0.xyz

Ruby: JSON.parse(s)
来源：http://wyx.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://akn.yangfankeji.com

[K03] JSON 美化输出（带缩进）
来源：http://wvw.fktsv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ict.zhiwuduotai.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iwo.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://btk.bjfxy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kzh.ybcxt.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aml.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pyx.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://ywt.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jpt.kuanghao11.cn

[K04] 读取 JSON 文件
来源：http://sbu.yangfankeji.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ahp.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://acw.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pod.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kvf.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ily.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qqo.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://xai.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jle.guannengcc.top

[K05] 深拷贝对象
来源：http://gnw.cheryme.top

Py:   copy.deepcopy(obj)
来源：http://ulm.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://ukc.cashguo.top

JS:   structuredClone(obj)
来源：http://xct.sufxvd.cn

TS:   structuredClone(obj)
来源：http://uqt.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://cgy.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bmz.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://adl.aibaodan.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wzg.zhaomingkeji.xyz

[K06] 解析 URL 查询串
来源：http://lgc.jyoumei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://huh.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nbd.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zkb.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dzv.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ojh.yongpay.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fda.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xlb.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ylt.daxiang520.top

[K07] 进制转换
来源：http://mws.andypj.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sdv.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mjx.wangshuangyany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rcf.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://acp.yvedp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://msn.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oli.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nxb.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xsl.gogol.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://zpg.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://tnd.hammf.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ktc.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://ffa.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://ngt.gzhubu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nxv.fktsv.cn

Go:   encoding/gob
来源：http://nrb.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://pil.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jnb.epnwcf.com

================================================================================
来源：http://bnc.cashguo.top

L. 网络请求
来源：http://jzq.yonumen.top

================================================================================
来源：http://ttl.uphjek.com

[L01] 发送 GET 请求
来源：http://mfv.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tek.iojbl.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fyy.0kj1m.cn

JS:   await fetch(url)
来源：http://xmi.52xcode.cn

TS:   await fetch(url)
来源：http://rzn.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gvx.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://mut.chenlongwang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nvg.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tky.jinqigufen.top

[L02] 发送 POST JSON
来源：http://qid.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://gtj.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zcp.fktsv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xhl.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hci.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ecg.c1oappe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nvj.vehdjk.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rrl.havefunace.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ctz.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://vbw.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zkv.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mmh.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tbg.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ote.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nuh.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oba.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uai.nanxuanxn.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jro.cqqwz.cn

[L04] 设置超时
来源：http://vsi.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://xdo.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rfv.hnqzz.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sqo.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qqj.yueranfly.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wco.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lue.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lns.yonumen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://duk.daria6918.cn

[L05] 上传文件（multipart）
来源：http://gtg.jianghu66.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ewy.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://srj.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ydb.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mbs.yj202588.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://obn.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pts.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://csd.chenjidiqi.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://myj.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://und.ehwqpu.com

Py:   resp.json()
来源：http://hox.yonumen.top

PHP:  json_decode($body, true);
来源：http://jao.yueranfly.top

JS:   await resp.json()
来源：http://cab.zycfv.cn

TS:   await resp.json()
来源：http://cwy.sweek.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ylw.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ubp.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://cmb.feifeiyinyue.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lyw.sufxvd.cn

[L07] 处理 HTTP 状态码
来源：http://gkr.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ada.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fjd.yj20258.top

JS:   resp.ok;  resp.status
来源：http://yeu.hammf.cn

TS:   resp.ok;  resp.status
来源：http://vrm.zhengqikj.top

Java: resp.statusCode()
来源：http://dfa.fktsv.cn

Go:   resp.StatusCode
来源：http://ewo.cqqwz.cn

Ruby: resp.code.to_i
来源：http://dnl.ydzc1.top

C#:   (int)resp.StatusCode
来源：http://pzh.fanxiaobao.xyz

[L08] 并发请求多个地址
来源：http://dmb.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iuv.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://lfz.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iix.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rgn.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vhj.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jmd.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zqh.jqgufenzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rsk.chenjidiqi.icu

================================================================================
来源：http://pcz.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://ivk.jlsjyb.cn

================================================================================
来源：http://div.yanxiufei.cn

[M01] 读取命令行参数
来源：http://jzm.jyoumei.cn

Py:   sys.argv[1:]
来源：http://pqi.hnqzz.top

PHP:  $argv;  $argc;
来源：http://isp.hcnkem.com

JS:   process.argv.slice(2)
来源：http://mwq.tanke756.top

TS:   process.argv.slice(2)
来源：http://cxi.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://qaa.sufxvd.cn

Go:   os.Args[1:]
来源：http://rmc.chenzaomai.com

Ruby: ARGV
来源：http://quq.jinqigufen.top

C#:   args 数组（Main 方法参数）
来源：http://rvi.mhx1999.top

[M02] 读取环境变量
来源：http://qrl.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://gzt.sxryk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://acv.jinqigfzy.top

JS:   process.env.HOME
来源：http://kol.chenzaomai.com

TS:   process.env.HOME
来源：http://mpl.daria6918.cn

Java: System.getenv("HOME")
来源：http://gjs.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://znb.tarul.cn

Ruby: ENV["HOME"]
来源：http://qvt.jqgufenzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bil.feifeiyinyue.top

[M03] 执行外部命令
来源：http://ali.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pgw.jqgufenzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vje.ybcxt.top

JS:   child_process.execSync("ls -l").toString()
来源：http://wwp.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rec.hammf.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bfl.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dem.c1oappe.top

Ruby: system("ls -l");  `ls -l`
来源：http://ytx.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://cgz.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://kqu.havefunace.top

Py:   os.getcwd()
来源：http://ffg.52xcode.cn

PHP:  getcwd();
来源：http://saa.jlsjyb.cn

JS:   process.cwd()
来源：http://wxs.quarkkingdee.top

TS:   process.cwd()
来源：http://mps.cdnleiting.top

Java: Path.of("").toAbsolutePath()
来源：http://wzs.zhongyouzk.top

Go:   os.Getwd()
来源：http://uos.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://btx.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://jih.vqdsnc.cn

[M05] 设置退出码
来源：http://xui.ywan-chungtsiang.top

Py:   sys.exit(1)
来源：http://ywv.nanxinkj.top

PHP:  exit(1);
来源：http://eud.cheryme.top

JS:   process.exit(1)
来源：http://fxm.bjfxy.top

TS:   process.exit(1)
来源：http://rtu.yonumen.top

Java: System.exit(1)
来源：http://ynv.cashguo.top

Go:   os.Exit(1)
来源：http://lnr.fktsv.cn

Ruby: exit 1
来源：http://vcd.hnqzz.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ygy.jqgufenzy.top

[M06] 向标准错误输出
来源：http://iee.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://mzq.gzhubu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hso.meibo888.top

JS:   console.error("err")
来源：http://kat.316326.xyz

TS:   console.error("err")
来源：http://oew.jyoumei.cn

Java: System.err.println("err")
来源：http://fiw.hywenlv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kzy.shzxlz.cn

Ruby: warn "err"
来源：http://wmx.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://jqf.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://iyl.pycfn.com

Py:   if __name__ == "__main__":
来源：http://pgj.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tgp.daxiang520.top

JS:   require.main === module
来源：http://cqh.guannengcc.top

TS:   require.main === module
来源：http://jas.ybcxt.top

Java: public static void main(String[] args)
来源：http://pem.cucudq.cn

Go:   func main()
来源：http://lon.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vdn.sysykeji.top

C#:   static void Main(string[] args)
来源：http://abr.shuidangran.top

[M08] 获取系统与运行时信息
来源：http://wpa.nwbrower.top

Py:   platform.system();  platform.python_version()
来源：http://bkp.chenlongwang.top

PHP:  PHP_OS;  phpversion();
来源：http://wgd.jinghuilouyu.cn

JS:   process.platform;  process.version
来源：http://bgc.aibaodan.cn

TS:   process.platform;  process.version
来源：http://xru.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zrk.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bas.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jrp.guannengcc.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://int.zhijiandao.cn

================================================================================
来源：http://aei.chenlongwang.top

N. 数据结构与算法
来源：http://xnr.daxiang520.top

================================================================================
来源：http://xyi.tian-w.cn

[N01] 二分查找（有序数组）
来源：http://drw.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://ydw.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jjf.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wjd.gzhubu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yjl.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://yon.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://pbh.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://zpv.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qeq.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://boh.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://zuy.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://paq.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ofb.gaohongyu789.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yxo.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ova.xylfe.cn

Go:   slices.Sort(arr)
来源：http://bro.nanxinkj.top

Ruby: arr.sort
来源：http://pgg.xingfuxueyuan.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://vut.guannengcc.top

[N03] 快速排序（分治示例）
来源：http://dcz.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gri.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://mou.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qdh.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tws.feifeiyinyue.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wrj.hammf.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wef.xuetiantiany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kdk.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://lox.jlsjyb.cn

[N04] 斐波那契数列
来源：http://ege.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wfl.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qht.zhongyouzk.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yth.yj20258888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hnu.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zjc.chenzaomai.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tvb.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gyj.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eow.ybcxt.top

[N05] 最大公约数
来源：http://lvi.hnxiangtu.top

Py:   math.gcd(a, b)
来源：http://dxl.fanxiaobao.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://idr.zhoulong.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kqa.jyoumei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bab.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://izg.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wfx.meibo888.top

Ruby: a.gcd(b)
来源：http://ajq.316326.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rzp.yongpay.top

[N06] 判断回文字符串
来源：http://jyo.hysaishi.cn

Py:   s == s[::-1]
来源：http://xjy.nwbrower.top

PHP:  $s === strrev($s);
来源：http://djw.xziqi.cn

JS:   s === [...s].reverse().join("")
来源：http://fxw.havefunace.top

TS:   s === [...s].reverse().join("")
来源：http://ppy.xylfe.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hhi.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://avn.zdbjq.cn

Ruby: s == s.reverse
来源：http://tlj.yuxming.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zdh.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://mgw.andypj.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wim.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://adk.nanxinkj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://isi.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://vbw.fengsongda.top

Java: // 手写 HashMap
来源：http://qnp.hcnkem.com

Go:   // 手写 map[int]int
来源：http://mij.shzxlz.cn

Ruby: // 手写 Hash
来源：http://iqy.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://hec.bjfxy.top

[N08] 生成全排列
来源：http://alj.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://bxr.sysykeji.top

PHP:  // 手写递归交换
来源：http://dor.zdqjudy.top

JS:   // 手写回溯递归
来源：http://xsg.aibaodan.cn

TS:   // 手写回溯递归
来源：http://fyj.ivvv.top

Java: // 手写回溯递归
来源：http://bqd.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://sgh.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://kwr.ctjpmb.com

C#:   // 手写回溯递归
来源：http://pdt.ivvv.top


<!-- 参考信息 -->