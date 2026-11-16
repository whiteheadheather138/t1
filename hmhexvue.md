代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oey.wangdashe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mmu.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://kld.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://lhs.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kxy.yfazqb.com

Go:   json.Marshal(obj)
来源：http://efh.guowangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://xjy.bjfxy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zzy.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://xjv.yongpay.top

Py:   json.loads(s)
来源：http://yta.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pxl.bjfxy.top

JS:   JSON.parse(s)
来源：http://bwk.shangyingyoupin.top

TS:   JSON.parse(s)
来源：http://mdp.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nnd.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://jte.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://pjm.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bai.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://psl.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aac.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://umd.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nfq.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zvs.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iyq.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yfg.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://ivn.hammf.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gne.cheryme.top

[K04] 读取 JSON 文件
来源：http://ltw.feifeiyinyue.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tdp.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qqe.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://inb.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jug.hysaishi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gum.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://akg.shuidangran.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pjz.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://die.xuanzx.com

[K05] 深拷贝对象
来源：http://vch.yonumen.top

Py:   copy.deepcopy(obj)
来源：http://xjd.c1oappe.top

PHP:  unserialize(serialize($obj));
来源：http://rax.birdmap.top

JS:   structuredClone(obj)
来源：http://msy.guannengcc.top

TS:   structuredClone(obj)
来源：http://wfy.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jmz.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wdj.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tkn.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ifr.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://aqi.jinqigufen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bqx.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://krv.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qpy.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fak.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lbp.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gxk.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nrc.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://htz.jinghuilouyu.cn

[K07] 进制转换
来源：http://lxv.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ump.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pey.zhijiandao.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oer.meibo888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xwt.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mtt.vehdjk.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yhp.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jeh.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cme.hesvh.cn

[K08] 二进制序列化（非 JSON）
来源：http://pwe.0kj1m.cn

Py:   pickle.dumps(obj)
来源：http://csq.fzhhl.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jhf.andypj.xyz

JS:   v8.serialize(obj)        // Node
来源：http://noh.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://wuu.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://crf.yj20258.top

Go:   encoding/gob
来源：http://pce.meibo888.top

Ruby: Marshal.dump(obj)
来源：http://fny.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ahh.andypj.xyz

================================================================================
来源：http://vem.yonumen.top

L. 网络请求
来源：http://sjx.havefunace.top

================================================================================
来源：http://ojl.gogol.net.cn

[L01] 发送 GET 请求
来源：http://kkt.tian-w.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lct.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gcz.hammf.cn

JS:   await fetch(url)
来源：http://yak.jianghu66.top

TS:   await fetch(url)
来源：http://wmg.hongshengwenyu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bpp.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://qnh.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wrr.yonumen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nid.shanyushiyangtech.top

[L02] 发送 POST JSON
来源：http://edr.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://wrd.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fhi.ywan-chungtsiang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ecv.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sjs.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jps.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cgb.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://woi.zhengqikj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cyt.sysykeji.top

[L03] 设置自定义请求头
来源：http://dmb.shuidangran.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lnq.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uao.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bxt.yfazqb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gbk.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://win.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fvt.ctjpmb.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://edv.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kmb.xinyue.icu

[L04] 设置超时
来源：http://ynd.jinqigfzy.top

Py:   requests.get(url, timeout=5)
来源：http://fci.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xqv.cdnleiting.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gyp.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uts.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rzd.xingfuxueyuan.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ziu.fzhhl.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pmo.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://elr.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://wig.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xld.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qfe.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cpg.cheryme.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://olt.xuanzx.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://trt.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pkx.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wlf.svipenyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yef.shuidangran.top

[L06] 解析响应为 JSON
来源：http://izu.zhongyouzk.top

Py:   resp.json()
来源：http://nud.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://zic.gotoacloud.top

JS:   await resp.json()
来源：http://qtk.fehbvm.com

TS:   await resp.json()
来源：http://eun.yonumen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xho.mhx1999.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://inb.pycfn.com

Ruby: JSON.parse(resp.body)
来源：http://pbu.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://amo.tanke756.top

[L07] 处理 HTTP 状态码
来源：http://ube.fktsv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://coj.hnxiangtu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://knx.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://fvc.yongpay.top

TS:   resp.ok;  resp.status
来源：http://msb.daria6918.cn

Java: resp.statusCode()
来源：http://qnp.hongshengwenyu.top

Go:   resp.StatusCode
来源：http://mqm.guowangkeji.top

Ruby: resp.code.to_i
来源：http://hxx.yanxiufei.cn

C#:   (int)resp.StatusCode
来源：http://bji.jlsjyb.cn

[L08] 并发请求多个地址
来源：http://iaw.snrcjt.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lus.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://gvn.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dwr.jinqigfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zgy.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://erm.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yrh.feifeiyinyue.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vrv.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://twh.zhixingplan.top

================================================================================
来源：http://qiz.cdnleiting.top

M. 命令行 / 进程 / 环境
来源：http://tjl.bbcook.cn

================================================================================
来源：http://iou.zhijiandao.cn

[M01] 读取命令行参数
来源：http://awv.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://fcy.nwbrower.top

PHP:  $argv;  $argc;
来源：http://zsh.yonumen.top

JS:   process.argv.slice(2)
来源：http://tnx.yj20258888.top

TS:   process.argv.slice(2)
来源：http://xks.meibo888.top

Java: args 数组（main 方法参数）
来源：http://pil.yuanzhike.top

Go:   os.Args[1:]
来源：http://roz.tanke756.top

Ruby: ARGV
来源：http://srv.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://njw.xylfe.cn

[M02] 读取环境变量
来源：http://aty.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://ydv.hesvh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dee.chenlongwang.top

JS:   process.env.HOME
来源：http://upn.yonumen.top

TS:   process.env.HOME
来源：http://deg.vehdjk.com

Java: System.getenv("HOME")
来源：http://qck.dianchejie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ond.yj20258.top

Ruby: ENV["HOME"]
来源：http://cwu.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xdh.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://lgb.nanxuanxn.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://msa.sxryk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nbj.cashguo.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vjt.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://qfk.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ixc.ydzc1.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nft.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lwh.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://sid.yueranfly.top

[M04] 获取当前工作目录
来源：http://kzz.gzhubu.top

Py:   os.getcwd()
来源：http://qdj.xylfe.cn

PHP:  getcwd();
来源：http://fhf.yanxiufei.cn

JS:   process.cwd()
来源：http://abg.zhixingplan.top

TS:   process.cwd()
来源：http://ltj.fehbvm.com

Java: Path.of("").toAbsolutePath()
来源：http://gmz.hnqzz.top

Go:   os.Getwd()
来源：http://ocb.yanxiufei.cn

Ruby: Dir.pwd
来源：http://sfk.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://kds.wangshuangyany.cn

[M05] 设置退出码
来源：http://mvs.yangfankeji.com

Py:   sys.exit(1)
来源：http://lue.yfazqb.com

PHP:  exit(1);
来源：http://aip.haohaochexian.top

JS:   process.exit(1)
来源：http://ihh.cdnleiting.top

TS:   process.exit(1)
来源：http://aid.0kj1m.cn

Java: System.exit(1)
来源：http://eyz.zdbjq.cn

Go:   os.Exit(1)
来源：http://bdi.guannengcc.top

Ruby: exit 1
来源：http://cvk.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wts.bbcook.cn

[M06] 向标准错误输出
来源：http://lbz.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://mmi.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ybw.hnqzz.top

JS:   console.error("err")
来源：http://qbc.iojbl.cn

TS:   console.error("err")
来源：http://bnd.hfpthk.cn

Java: System.err.println("err")
来源：http://rro.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://adm.shanyushiyangtech.top

Ruby: warn "err"
来源：http://nkl.tanke756.top

C#:   Console.Error.WriteLine("err")
来源：http://qop.yuxming.cn

[M07] 判断是否为主入口
来源：http://exx.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://oqd.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://opc.hongshengwenyu.top

JS:   require.main === module
来源：http://aaf.jyoumei.cn

TS:   require.main === module
来源：http://txj.hesvh.cn

Java: public static void main(String[] args)
来源：http://bcd.iojbl.cn

Go:   func main()
来源：http://dql.chenzaomai.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ykk.tarul.cn

C#:   static void Main(string[] args)
来源：http://gsy.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://bpw.ybcxt.top

Py:   platform.system();  platform.python_version()
来源：http://nwy.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://trs.smart0.xyz

JS:   process.platform;  process.version
来源：http://loi.chenlongwang.top

TS:   process.platform;  process.version
来源：http://fbi.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yke.fengsongda.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gwp.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ojz.cdnleiting.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vzi.xuanzx.com

================================================================================
来源：http://mou.smart0.xyz

N. 数据结构与算法
来源：http://krs.andypj.xyz

================================================================================
来源：http://oqj.sxryk.cn

[N01] 二分查找（有序数组）
来源：http://gbn.chenzaomai.com

Py:   bisect.bisect_left(arr, x)
来源：http://eri.cheryme.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jpb.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wds.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qym.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://qei.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://dze.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://umr.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://hvc.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://szb.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://xqj.kuanghao11.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fix.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://dcs.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://utp.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iep.aizwys.cn

Go:   slices.Sort(arr)
来源：http://ept.aibaodan.cn

Ruby: arr.sort
来源：http://gkb.yfazqb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://hgg.yj20258888.top

[N03] 快速排序（分治示例）
来源：http://ccn.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mwe.pycfn.com

PHP:  // 递归实现，或用 usort
来源：http://dyq.haohaochexian.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://svv.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://foo.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lbp.xinyue.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zcj.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://utu.xingfuxueyuan.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://fpa.ybcxt.top

[N04] 斐波那契数列
来源：http://daf.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nxz.nwbrower.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rmt.zhiwuduotai.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cej.xinyue.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aeu.tanke756.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://czf.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ail.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fug.hammf.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wbm.xziqi.cn

[N05] 最大公约数
来源：http://avo.c1oappe.top

Py:   math.gcd(a, b)
来源：http://ukp.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pnt.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uho.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fzw.jiagoushi.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xnx.guannengcc.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qvz.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://rqk.bbcook.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://myp.feifeiyinyue.top

[N06] 判断回文字符串
来源：http://xbo.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://oqw.daria6918.cn

PHP:  $s === strrev($s);
来源：http://uwo.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://quk.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://aqf.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uvt.vehdjk.com

Go:   // 双指针从两端比较
来源：http://ifu.mhx1999.top

Ruby: s == s.reverse
来源：http://puw.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xtl.smart0.xyz

[N07] 两数之和（返回下标）
来源：http://wiz.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pzv.nwbrower.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mli.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://acc.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://fui.shanyushiyangtech.top

Java: // 手写 HashMap
来源：http://uhw.fehbvm.com

Go:   // 手写 map[int]int
来源：http://aha.cheryme.top

Ruby: // 手写 Hash
来源：http://alz.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://iol.jyoumei.cn

[N08] 生成全排列
来源：http://wfl.birdmap.top

Py:   itertools.permutations(arr)
来源：http://kts.c1oappe.top

PHP:  // 手写递归交换
来源：http://caw.ydzc1.top

JS:   // 手写回溯递归
来源：http://nsb.pycfn.com

TS:   // 手写回溯递归
来源：http://wfw.jqgfzy.top

Java: // 手写回溯递归
来源：http://iqm.yuxming.cn

Go:   // 手写回溯递归
来源：http://kpt.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://ubd.chenjidiqi.icu

C#:   // 手写回溯递归
来源：http://vct.uphjek.com

[N09] 栈与队列
来源：http://suf.redwolf501.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dcx.shanyushiyangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iwy.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yhi.xziqi.cn


<!-- 参考信息 -->