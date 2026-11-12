代发 wailian999

================================================================================
来源：http://all.sxryk.cn

K. JSON 与序列化
来源：http://tbt.jqgufenzy.top

================================================================================
来源：http://zsv.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://drv.zhiwuduotai.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://feq.cheryme.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pui.yuxming.cn

JS:   JSON.stringify(obj)
来源：http://cbk.ppjwa.cn

TS:   JSON.stringify(obj)
来源：http://vxt.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pge.hnxiangtu.top

Go:   json.Marshal(obj)
来源：http://yvr.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://chu.bbcook.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ctj.hesvh.cn

[K02] JSON 字符串转对象
来源：http://ogs.daria6918.cn

Py:   json.loads(s)
来源：http://bcv.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ymv.fktsv.cn

JS:   JSON.parse(s)
来源：http://acv.jqgufenzy.top

TS:   JSON.parse(s)
来源：http://hxn.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fsy.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://mon.ywan-chungtsiang.top

Ruby: JSON.parse(s)
来源：http://qvo.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bxp.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://tpf.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yil.chenlongwang.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gmo.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fui.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ujl.hfpthk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yfj.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hzf.cheryme.top

Ruby: JSON.pretty_generate(obj)
来源：http://bqt.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rzt.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://whn.ydzc1.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://utj.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://whw.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jll.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vrp.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ctm.aibaodan.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ceg.sweek.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dqw.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mdt.fengsongda.top

[K05] 深拷贝对象
来源：http://pra.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://xzu.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://sut.yonumen.top

JS:   structuredClone(obj)
来源：http://icq.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://kgu.xinyue.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://paz.daria6918.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://apj.sweek.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aem.hnxiangtu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qqt.zhoulong.xyz

[K06] 解析 URL 查询串
来源：http://alo.fengsongda.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://stz.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://poh.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bdw.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ywh.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jlc.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xuo.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ohm.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zjr.shanyushiyangkeji.top

[K07] 进制转换
来源：http://nxh.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mck.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mhb.zhiwuduotai.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ets.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nrv.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vnq.zhongyouzk.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bjo.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yal.sweek.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tio.shuidangran.top

[K08] 二进制序列化（非 JSON）
来源：http://etq.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://hbb.jinghuilouyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qvs.wangdashe.top

JS:   v8.serialize(obj)        // Node
来源：http://utq.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://ziv.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wmj.ctjpmb.com

Go:   encoding/gob
来源：http://bnz.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://oqa.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mnc.cdnleiting.top

================================================================================
来源：http://tqw.svipenyu.cn

L. 网络请求
来源：http://hck.sjlbkw.cn

================================================================================
来源：http://lmx.sufxvd.cn

[L01] 发送 GET 请求
来源：http://nor.zhaomingkeji.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://chr.jiagoushi.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lfd.zhongyouzk.top

JS:   await fetch(url)
来源：http://wiq.kuanghao11.cn

TS:   await fetch(url)
来源：http://lkx.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nkc.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://ftv.jinyuanbaomall.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://twi.316326.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://evo.tianlin.xyz

[L02] 发送 POST JSON
来源：http://vip.jinqigufen.top

Py:   requests.post(url, json={"a": 1})
来源：http://yaz.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ddv.chenlongwang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wwh.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://krf.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zhb.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zix.zhengqikj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hig.gzhubu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nxi.cashguo.top

[L03] 设置自定义请求头
来源：http://nbb.ehwqpu.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pww.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nad.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ytl.wangdashe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nfk.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ejf.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vnj.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qyp.aizwys.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lak.9152youxi.cn

[L04] 设置超时
来源：http://nws.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://aax.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ffx.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yuw.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ztz.nanxinkj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kqo.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jnm.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yeg.pycfn.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xkg.nanxinkj.top

[L05] 上传文件（multipart）
来源：http://etx.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cch.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://abk.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sii.hfpthk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://joi.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dzi.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://enw.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lia.zhaomingkeji.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fap.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://aas.jqgfzy.top

Py:   resp.json()
来源：http://hwv.vehdjk.com

PHP:  json_decode($body, true);
来源：http://qfg.chenlongwang.top

JS:   await resp.json()
来源：http://wab.yuxming.cn

TS:   await resp.json()
来源：http://gzl.fehbvm.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pcs.meibo888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sik.jianghu66.top

Ruby: JSON.parse(resp.body)
来源：http://ooj.cqqwz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lef.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://wdv.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sgr.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mpi.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://mdl.quarkkingdee.top

TS:   resp.ok;  resp.status
来源：http://czr.yuxming.cn

Java: resp.statusCode()
来源：http://pbf.shangyingyoupin.top

Go:   resp.StatusCode
来源：http://vyr.zycfv.cn

Ruby: resp.code.to_i
来源：http://vds.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://mrp.shzxlz.cn

[L08] 并发请求多个地址
来源：http://jgv.aibaodan.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://idp.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://hsr.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zkj.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xou.hywenlv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wgy.kuanghao11.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fmc.fehbvm.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lmg.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://job.aibaodan.cn

================================================================================
来源：http://cmp.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://ldv.jianghu66.top

================================================================================
来源：http://uub.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://xqy.daxiang520.top

Py:   sys.argv[1:]
来源：http://ufc.smart0.xyz

PHP:  $argv;  $argc;
来源：http://tyw.gzhubu.top

JS:   process.argv.slice(2)
来源：http://ren.xziqi.cn

TS:   process.argv.slice(2)
来源：http://adx.iojbl.cn

Java: args 数组（main 方法参数）
来源：http://enp.jiagoushi.top

Go:   os.Args[1:]
来源：http://qvy.ywan-chungtsiang.top

Ruby: ARGV
来源：http://ahg.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://kll.yj20258.top

[M02] 读取环境变量
来源：http://bgi.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://dpj.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gbm.guannengcc.top

JS:   process.env.HOME
来源：http://bum.guannengcc.top

TS:   process.env.HOME
来源：http://yiy.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://pvt.fktsv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nnb.pengpengdd.cyou

Ruby: ENV["HOME"]
来源：http://esa.zdbjq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xgw.yj20258888.top

[M03] 执行外部命令
来源：http://xdw.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mak.yfazqb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cxf.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://oin.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://ach.daxiang520.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://idk.ctjpmb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://rav.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://tnz.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://nzy.daria6918.cn

[M04] 获取当前工作目录
来源：http://smj.ydzc1.top

Py:   os.getcwd()
来源：http://xwq.iojbl.cn

PHP:  getcwd();
来源：http://lrc.sweek.top

JS:   process.cwd()
来源：http://jff.sufxvd.cn

TS:   process.cwd()
来源：http://for.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://bmz.zhijiandao.cn

Go:   os.Getwd()
来源：http://cwg.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://pxo.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ahm.zhiwuduotai.top

[M05] 设置退出码
来源：http://jjc.yonumen.top

Py:   sys.exit(1)
来源：http://qxz.yj20258.top

PHP:  exit(1);
来源：http://ipm.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://snu.zdqjudy.top

TS:   process.exit(1)
来源：http://tbn.yj20258888.top

Java: System.exit(1)
来源：http://syu.hcnkem.com

Go:   os.Exit(1)
来源：http://jqd.yj20258.top

Ruby: exit 1
来源：http://fsm.tarul.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bhz.vehdjk.com

[M06] 向标准错误输出
来源：http://pdo.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://nwz.zhongyouzk.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mau.vqdsnc.cn

JS:   console.error("err")
来源：http://tog.havefunace.top

TS:   console.error("err")
来源：http://cgz.hysaishi.cn

Java: System.err.println("err")
来源：http://hdl.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iqr.yongpay.top

Ruby: warn "err"
来源：http://zav.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://lsr.ivvv.top

[M07] 判断是否为主入口
来源：http://kcu.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://xsm.sweek.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://szh.jqgufenzy.top

JS:   require.main === module
来源：http://rpw.cqqwz.cn

TS:   require.main === module
来源：http://ezx.gzhubu.top

Java: public static void main(String[] args)
来源：http://muq.gzhubu.top

Go:   func main()
来源：http://sqi.bjfxy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pku.xinyue.icu

C#:   static void Main(string[] args)
来源：http://tzu.mhx1999.top

[M08] 获取系统与运行时信息
来源：http://bpo.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://iii.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ade.jyoumei.cn

JS:   process.platform;  process.version
来源：http://nmk.zdbjq.cn

TS:   process.platform;  process.version
来源：http://cqw.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://urg.andypj.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://voq.fzhhl.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zzs.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uuk.gogol.net.cn

================================================================================
来源：http://gll.nanxuanxn.top

N. 数据结构与算法
来源：http://dec.aizwys.cn

================================================================================
来源：http://irw.tanke756.top

[N01] 二分查找（有序数组）
来源：http://fda.sweek.top

Py:   bisect.bisect_left(arr, x)
来源：http://jwn.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jvd.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://owm.sjlbkw.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gbs.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://mka.redwolf501.top

Go:   sort.SearchInts(arr, x)
来源：http://zcs.zhixingplan.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://unb.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://mqf.fzhhl.top

[N02] 排序（工程实践用内置实现）
来源：http://vzf.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://lox.c1oappe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://psu.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tlx.nwbrower.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fjn.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tkn.hfpthk.cn

Go:   slices.Sort(arr)
来源：http://jox.fengsongda.top

Ruby: arr.sort
来源：http://kok.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://afg.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://hoh.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hza.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://mbn.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tkb.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vfd.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gno.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://olb.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ngu.sweek.top

C#:   // 手写递归，或 Array.Sort
来源：http://gav.zhengqikj.top

[N04] 斐波那契数列
来源：http://tom.yfazqb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zld.hesvh.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ovj.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mry.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cvm.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jmj.hongshengwenyu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qsy.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rcv.jinqigufen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://stw.fzhhl.top

[N05] 最大公约数
来源：http://vgn.fehbvm.com

Py:   math.gcd(a, b)
来源：http://osf.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wje.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hzy.tian-w.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://khn.yonumen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://scp.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ofe.pycfn.com

Ruby: a.gcd(b)
来源：http://don.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iie.hcnkem.com

[N06] 判断回文字符串
来源：http://sxv.yfazqb.com

Py:   s == s[::-1]
来源：http://xvt.gogol.net.cn

PHP:  $s === strrev($s);
来源：http://vcj.yj20258888.top

JS:   s === [...s].reverse().join("")
来源：http://ezp.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://xir.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mgu.fzhhl.top

Go:   // 双指针从两端比较
来源：http://vpx.jyoumei.cn

Ruby: s == s.reverse
来源：http://yuj.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lvl.jinyuanbaomall.cn

[N07] 两数之和（返回下标）
来源：http://hac.pycfn.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qku.sweek.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vnc.aibaodan.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://whd.hnqzz.top

TS:   // 手写 Map<string, number>
来源：http://sbf.mhx1999.top

Java: // 手写 HashMap
来源：http://szr.xingfuxueyuan.xyz

Go:   // 手写 map[int]int
来源：http://dtd.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://dwr.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://uwv.cdnleiting.top

[N08] 生成全排列
来源：http://nsl.birdmap.top

Py:   itertools.permutations(arr)
来源：http://ewp.iojbl.cn

PHP:  // 手写递归交换
来源：http://pue.meibo888.top

JS:   // 手写回溯递归
来源：http://pjf.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://lms.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://qvv.snrcjt.cn

Go:   // 手写回溯递归
来源：http://rcc.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://uut.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://giw.ydjk.org.cn


<!-- 参考信息 -->