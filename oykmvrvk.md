代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yyd.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://mwt.gotoacloud.top

Ruby: obj.to_json                                     // require "json"
来源：http://ffi.meibo888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://umr.sxryk.cn

[K02] JSON 字符串转对象
来源：http://dkr.chenjidiqi.icu

Py:   json.loads(s)
来源：http://zae.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jfi.iojbl.cn

JS:   JSON.parse(s)
来源：http://uzu.yuxming.cn

TS:   JSON.parse(s)
来源：http://ciq.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ckk.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://ott.yangfankeji.com

Ruby: JSON.parse(s)
来源：http://kmo.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://was.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://qnx.hfpthk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kzk.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hmy.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yxf.iojbl.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://npt.zhiwuduotai.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://khi.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hvi.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kao.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xzd.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://vjv.ydjk.org.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tpm.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eqe.wangdashe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vgy.52xcode.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://amr.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mjc.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yjp.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ufl.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jto.epnwcf.com

[K05] 深拷贝对象
来源：http://rap.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://iun.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://sfv.sweek.top

JS:   structuredClone(obj)
来源：http://lsb.svipenyu.cn

TS:   structuredClone(obj)
来源：http://zhn.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sgq.jinyuanbaomall.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rcb.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qel.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://uqz.yanxiufei.cn

[K06] 解析 URL 查询串
来源：http://jbe.yuxming.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hli.gzhubu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mmx.svipenyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wzt.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mir.gogol.net.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bgw.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nrq.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vbj.svipenyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dtk.yfazqb.com

[K07] 进制转换
来源：http://gkg.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kwv.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://idf.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zrf.zdqjudy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eaf.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://idu.hywenlv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qcd.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eoh.yuanzhike.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nad.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://xdo.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://bht.wangshuangyany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://egj.iojbl.cn

JS:   v8.serialize(obj)        // Node
来源：http://tzb.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://jlr.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://exo.tian-w.cn

Go:   encoding/gob
来源：http://mrm.shuidangran.top

Ruby: Marshal.dump(obj)
来源：http://emr.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fbw.yj20258888.top

================================================================================
来源：http://ofg.havefunace.top

L. 网络请求
来源：http://eqk.zycfv.cn

================================================================================
来源：http://ggz.aibaodan.cn

[L01] 发送 GET 请求
来源：http://jwg.dashuyun.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wrk.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ttl.zycfv.cn

JS:   await fetch(url)
来源：http://jtm.tian-w.cn

TS:   await fetch(url)
来源：http://xxq.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hqe.guannengcc.top

Go:   resp, err := http.Get(url)
来源：http://sez.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lxv.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gwg.gotoacloud.top

[L02] 发送 POST JSON
来源：http://hsh.fanxiaobao.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://tga.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jmy.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zft.sweek.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oqo.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dtp.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pgm.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hym.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://itg.yvedp.cn

[L03] 设置自定义请求头
来源：http://bwh.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://srt.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jwb.52xcode.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://elg.xuanzx.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wrs.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mfe.yj20258.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://btk.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yyv.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wvc.yongpay.top

[L04] 设置超时
来源：http://mfb.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://hxo.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sou.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nda.jinqigufen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uie.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ene.daxiang520.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cst.zhoulong.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fpi.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vxv.sxryk.cn

[L05] 上传文件（multipart）
来源：http://kwq.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jzx.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wis.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mfu.yfazqb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dge.hnxiangtu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fdn.bbcook.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://biy.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mjl.yj202588.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ynf.xinyue.icu

[L06] 解析响应为 JSON
来源：http://kgv.0kj1m.cn

Py:   resp.json()
来源：http://rus.pycfn.com

PHP:  json_decode($body, true);
来源：http://ykv.birdmap.top

JS:   await resp.json()
来源：http://frm.hongshengwenyu.top

TS:   await resp.json()
来源：http://yam.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lmq.jlsjyb.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ten.ydjk.org.cn

Ruby: JSON.parse(resp.body)
来源：http://ufu.ydjk.org.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vop.shanyushiyangtech.top

[L07] 处理 HTTP 状态码
来源：http://tfn.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rlq.ivvv.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vll.xinyue.icu

JS:   resp.ok;  resp.status
来源：http://tzp.cheryme.top

TS:   resp.ok;  resp.status
来源：http://epc.yj20258.top

Java: resp.statusCode()
来源：http://gfg.nanxinkj.top

Go:   resp.StatusCode
来源：http://nel.tian-w.cn

Ruby: resp.code.to_i
来源：http://xsb.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://rwp.ehwqpu.com

[L08] 并发请求多个地址
来源：http://pan.andypj.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tsp.cqqwz.cn

PHP:  curl_multi_init() 系列
来源：http://njw.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://szw.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bau.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://odl.hfpthk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://laf.havefunace.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dvs.zdbjq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dhr.hammf.cn

================================================================================
来源：http://bfh.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://siz.pycfn.com

================================================================================
来源：http://rbk.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://krn.haohaochexian.top

Py:   sys.argv[1:]
来源：http://luu.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://dno.shuidangran.top

JS:   process.argv.slice(2)
来源：http://pef.ppjwa.cn

TS:   process.argv.slice(2)
来源：http://jkd.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://dex.sufxvd.cn

Go:   os.Args[1:]
来源：http://ibu.hnxiangtu.top

Ruby: ARGV
来源：http://wnp.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://nuv.pengpengdd.cyou

[M02] 读取环境变量
来源：http://uny.sjlbkw.cn

Py:   os.environ.get("HOME")
来源：http://hxo.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zss.hysaishi.cn

JS:   process.env.HOME
来源：http://pgx.epnwcf.com

TS:   process.env.HOME
来源：http://ime.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://llf.aizwys.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://guo.zhijiandao.cn

Ruby: ENV["HOME"]
来源：http://zfb.jlsjyb.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tmm.316326.xyz

[M03] 执行外部命令
来源：http://yvs.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fut.jqgufenzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eon.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lhx.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://eev.gzhubu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mgn.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://osu.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://bxq.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://fmu.cucudq.cn

[M04] 获取当前工作目录
来源：http://klw.zhengqikj.top

Py:   os.getcwd()
来源：http://lfb.shangyingyoupin.top

PHP:  getcwd();
来源：http://rdo.chenjidiqi.icu

JS:   process.cwd()
来源：http://ppa.bbcook.cn

TS:   process.cwd()
来源：http://lto.aizwys.cn

Java: Path.of("").toAbsolutePath()
来源：http://wak.yongpay.top

Go:   os.Getwd()
来源：http://hrx.yonumen.top

Ruby: Dir.pwd
来源：http://voz.jinqigfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://pte.cdnleiting.top

[M05] 设置退出码
来源：http://ruu.hnqzz.top

Py:   sys.exit(1)
来源：http://hfz.yuanzhike.top

PHP:  exit(1);
来源：http://cuu.gzhubu.top

JS:   process.exit(1)
来源：http://gnx.andypj.xyz

TS:   process.exit(1)
来源：http://dqu.jianghu66.top

Java: System.exit(1)
来源：http://xgy.jlsjyb.cn

Go:   os.Exit(1)
来源：http://syr.epnwcf.com

Ruby: exit 1
来源：http://dod.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ase.vehdjk.com

[M06] 向标准错误输出
来源：http://evp.yvedp.cn

Py:   print("err", file=sys.stderr)
来源：http://cyy.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hto.ivvv.top

JS:   console.error("err")
来源：http://izq.yueranfly.top

TS:   console.error("err")
来源：http://xxu.gogol.net.cn

Java: System.err.println("err")
来源：http://rgn.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://czw.smart0.xyz

Ruby: warn "err"
来源：http://aag.gotoacloud.top

C#:   Console.Error.WriteLine("err")
来源：http://eed.nanxuanxn.top

[M07] 判断是否为主入口
来源：http://zkz.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://zax.haohaochexian.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://thv.xuanzx.com

JS:   require.main === module
来源：http://rzr.zhijiandao.cn

TS:   require.main === module
来源：http://xho.chenzaomai.com

Java: public static void main(String[] args)
来源：http://psk.fanxiaobao.xyz

Go:   func main()
来源：http://wgi.gogol.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jkg.hammf.cn

C#:   static void Main(string[] args)
来源：http://cqs.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://dvt.zdbjq.cn

Py:   platform.system();  platform.python_version()
来源：http://nty.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://goa.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://amf.fktsv.cn

TS:   process.platform;  process.version
来源：http://nww.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vwn.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zfd.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hea.0kj1m.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://glc.haohaochexian.top

================================================================================
来源：http://dep.hysaishi.cn

N. 数据结构与算法
来源：http://jhw.aibaodan.cn

================================================================================
来源：http://vwq.yonumen.top

[N01] 二分查找（有序数组）
来源：http://ech.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://vhy.uphjek.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lav.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zmx.sufxvd.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nws.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://svc.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://ssp.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gdd.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ygt.quarkkingdee.top

[N02] 排序（工程实践用内置实现）
来源：http://jcr.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://qog.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nxy.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gqu.tanke756.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lkp.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uaa.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://oka.hywenlv.cn

Ruby: arr.sort
来源：http://qyl.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pyi.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://ugm.jinqigfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rfg.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://xnc.gotoacloud.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tep.chenzaomai.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wjq.tian-w.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://phr.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rrm.daxiang520.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ckq.sweek.top

C#:   // 手写递归，或 Array.Sort
来源：http://sau.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://bav.daxiang520.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ubz.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jby.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ukc.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pjx.zycfv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yau.ehwqpu.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yde.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mkl.jyoumei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zrp.xuetiantiany.cn

[N05] 最大公约数
来源：http://jrl.sufxvd.cn

Py:   math.gcd(a, b)
来源：http://hfn.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mls.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jci.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hrl.yuanzhike.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dls.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kkk.nwbrower.top

Ruby: a.gcd(b)
来源：http://cnk.havefunace.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kkz.yueranfly.top

[N06] 判断回文字符串
来源：http://vba.cashguo.top

Py:   s == s[::-1]
来源：http://jia.xuanzx.com

PHP:  $s === strrev($s);
来源：http://ych.gzhubu.top

JS:   s === [...s].reverse().join("")
来源：http://jtb.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://azc.hysaishi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qpj.sxryk.cn

Go:   // 双指针从两端比较
来源：http://lkd.hcnkem.com

Ruby: s == s.reverse
来源：http://flb.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jad.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://pry.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://abw.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jie.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xrn.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://kkk.xylfe.cn

Java: // 手写 HashMap
来源：http://wuh.cucudq.cn

Go:   // 手写 map[int]int
来源：http://yic.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://min.bbcook.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hcq.feifeiyinyue.top

[N08] 生成全排列
来源：http://sob.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://uyk.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://yyq.jinqigufen.top

JS:   // 手写回溯递归
来源：http://ueh.yangfankeji.com

TS:   // 手写回溯递归
来源：http://rhx.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://iqk.jyoumei.cn

Go:   // 手写回溯递归
来源：http://xoz.gotoacloud.top

Ruby: arr.permutation.to_a
来源：http://iuj.zhixingplan.top

C#:   // 手写回溯递归
来源：http://lou.xylfe.cn

[N09] 栈与队列
来源：http://bwg.havefunace.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yaz.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ayk.zhijiandao.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cvo.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://klg.gogol.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aqq.0kj1m.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ocq.shuidangran.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tyg.sysykeji.top


<!-- 参考信息 -->