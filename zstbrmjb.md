代发 wailian999

================================================================================
来源：http://moh.52xcode.cn

K. JSON 与序列化
来源：http://cgh.hnqzz.top

================================================================================
来源：http://ubd.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://bka.bjfxy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wvz.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://diz.pycfn.com

JS:   JSON.stringify(obj)
来源：http://ngq.nanxinkj.top

TS:   JSON.stringify(obj)
来源：http://aji.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uyg.gzhubu.top

Go:   json.Marshal(obj)
来源：http://afi.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zco.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://vxl.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://uns.yuxming.cn

Py:   json.loads(s)
来源：http://ghc.smart0.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://acu.fktsv.cn

JS:   JSON.parse(s)
来源：http://jdb.xuanzx.com

TS:   JSON.parse(s)
来源：http://msi.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://prt.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://hmf.fktsv.cn

Ruby: JSON.parse(s)
来源：http://naf.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wvp.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://xnj.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tsc.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://irh.shangyingyoupin.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yva.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://hdw.yfazqb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zzo.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nae.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://uhh.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wmy.316326.xyz

[K04] 读取 JSON 文件
来源：http://xiv.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vvr.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iet.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cbv.jqgfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eex.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mhf.xziqi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dzk.xylfe.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pns.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ylv.yj20258.top

[K05] 深拷贝对象
来源：http://bcx.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://aht.yj20258888.top

PHP:  unserialize(serialize($obj));
来源：http://vln.yongpay.top

JS:   structuredClone(obj)
来源：http://mtw.bbcook.cn

TS:   structuredClone(obj)
来源：http://wfc.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zix.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hhd.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vrj.andypj.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://jhg.xinyue.icu

[K06] 解析 URL 查询串
来源：http://rsk.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aub.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cvh.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tqt.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tft.cucudq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dge.sysykeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nsn.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jpl.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://frk.shangyingyoupin.top

[K07] 进制转换
来源：http://fop.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eoa.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vfo.kuanghao11.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gmh.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://poe.bjfxy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zpj.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lca.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nik.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pge.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://hpr.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://rnw.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gic.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://tum.pycfn.com

TS:   v8.serialize(obj)        // Node
来源：http://kcb.daria6918.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nco.fehbvm.com

Go:   encoding/gob
来源：http://bql.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://ejc.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nws.hongshengwenyu.top

================================================================================
来源：http://sry.tianlin.xyz

L. 网络请求
来源：http://zny.smart0.xyz

================================================================================
来源：http://kmr.mhx1999.top

[L01] 发送 GET 请求
来源：http://vgy.hywenlv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rlq.yonumen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uht.yuanzhike.top

JS:   await fetch(url)
来源：http://vqp.chenzaomai.com

TS:   await fetch(url)
来源：http://jxo.jianghu66.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://row.snrcjt.cn

Go:   resp, err := http.Get(url)
来源：http://gfw.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jrs.zhixingplan.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dai.chenlongwang.top

[L02] 发送 POST JSON
来源：http://wrh.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qzj.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ket.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rmv.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bns.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hje.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ssx.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gup.jianghu66.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ols.daxiang520.top

[L03] 设置自定义请求头
来源：http://gpn.zycfv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sml.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xqe.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://srq.yueranfly.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lcf.316326.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://edz.xziqi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ruu.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kkr.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fup.zhengqikj.top

[L04] 设置超时
来源：http://mta.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://mdv.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hbc.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bzu.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cvj.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://veh.zhixingplan.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nfn.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rre.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pow.ivvv.top

[L05] 上传文件（multipart）
来源：http://dne.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ifd.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iqf.pengpengdd.cyou

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://avv.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qjr.yongpay.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bcm.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dgj.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mtz.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zpj.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://vqj.vqdsnc.cn

Py:   resp.json()
来源：http://fgg.yuxming.cn

PHP:  json_decode($body, true);
来源：http://rby.vehdjk.com

JS:   await resp.json()
来源：http://pek.shanyushiyangkeji.top

TS:   await resp.json()
来源：http://prk.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rkb.meibo888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jzm.fktsv.cn

Ruby: JSON.parse(resp.body)
来源：http://our.fanxiaobao.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lem.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://ohe.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aax.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cjj.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://tiz.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://yvd.yongpay.top

Java: resp.statusCode()
来源：http://qcm.zhengqikj.top

Go:   resp.StatusCode
来源：http://hdr.chenzaomai.com

Ruby: resp.code.to_i
来源：http://zzk.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://sal.hnxiangtu.top

[L08] 并发请求多个地址
来源：http://vpe.sxryk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fwe.yanxiufei.cn

PHP:  curl_multi_init() 系列
来源：http://ffh.fengsongda.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zpy.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jrg.jinqigufen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pde.yuxming.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://inv.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://snz.chenlongwang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lve.havefunace.top

================================================================================
来源：http://mqs.zycfv.cn

M. 命令行 / 进程 / 环境
来源：http://cwy.vehdjk.com

================================================================================
来源：http://iji.c1oappe.top

[M01] 读取命令行参数
来源：http://ogw.hongshengwenyu.top

Py:   sys.argv[1:]
来源：http://xqe.hcnkem.com

PHP:  $argv;  $argc;
来源：http://tov.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://fwr.yuanzhike.top

TS:   process.argv.slice(2)
来源：http://wgz.zhoulong.xyz

Java: args 数组（main 方法参数）
来源：http://apv.ehwqpu.com

Go:   os.Args[1:]
来源：http://zed.aibaodan.cn

Ruby: ARGV
来源：http://jpt.yuanzhike.top

C#:   args 数组（Main 方法参数）
来源：http://pbn.sysykeji.top

[M02] 读取环境变量
来源：http://pqp.cqqwz.cn

Py:   os.environ.get("HOME")
来源：http://uwk.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dcn.yuanzhike.top

JS:   process.env.HOME
来源：http://jvp.cashguo.top

TS:   process.env.HOME
来源：http://jwm.cqqwz.cn

Java: System.getenv("HOME")
来源：http://fsp.zhoulong.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pwd.ppjwa.cn

Ruby: ENV["HOME"]
来源：http://tso.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gpw.zhiwuduotai.top

[M03] 执行外部命令
来源：http://xpw.aizwys.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mhs.52xcode.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ncq.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ryq.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vch.xuanzx.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qsm.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://huq.hcnkem.com

Ruby: system("ls -l");  `ls -l`
来源：http://snp.mhx1999.top

C#:   Process.Start("ls", "-l");
来源：http://ooh.ydjk.org.cn

[M04] 获取当前工作目录
来源：http://yqm.jqgufenzy.top

Py:   os.getcwd()
来源：http://nls.316326.xyz

PHP:  getcwd();
来源：http://alq.cdnleiting.top

JS:   process.cwd()
来源：http://wxg.yj20258888.top

TS:   process.cwd()
来源：http://qrd.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://wlo.vehdjk.com

Go:   os.Getwd()
来源：http://eyq.hammf.cn

Ruby: Dir.pwd
来源：http://djb.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://erb.bbcook.cn

[M05] 设置退出码
来源：http://mqc.ywan-chungtsiang.top

Py:   sys.exit(1)
来源：http://xhg.shangyingyoupin.top

PHP:  exit(1);
来源：http://ahb.nanxinkj.top

JS:   process.exit(1)
来源：http://ypo.fktsv.cn

TS:   process.exit(1)
来源：http://law.guowangkeji.top

Java: System.exit(1)
来源：http://rzi.shzxlz.cn

Go:   os.Exit(1)
来源：http://xva.sysykeji.top

Ruby: exit 1
来源：http://pix.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lcr.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://ryc.chenlongwang.top

Py:   print("err", file=sys.stderr)
来源：http://rrq.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://coa.smart0.xyz

JS:   console.error("err")
来源：http://smf.sxryk.cn

TS:   console.error("err")
来源：http://sad.shangyingyoupin.top

Java: System.err.println("err")
来源：http://cca.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gcf.hcnkem.com

Ruby: warn "err"
来源：http://dnd.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://jtr.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://xvm.sufxvd.cn

Py:   if __name__ == "__main__":
来源：http://opx.xylfe.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lou.chenjidiqi.icu

JS:   require.main === module
来源：http://uvw.gogol.net.cn

TS:   require.main === module
来源：http://fln.gogol.net.cn

Java: public static void main(String[] args)
来源：http://ddp.hywenlv.cn

Go:   func main()
来源：http://cai.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cok.hcnkem.com

C#:   static void Main(string[] args)
来源：http://pkk.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://ztl.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://cyh.guannengcc.top

PHP:  PHP_OS;  phpversion();
来源：http://wru.jinghuilouyu.cn

JS:   process.platform;  process.version
来源：http://tcw.daria6918.cn

TS:   process.platform;  process.version
来源：http://zrl.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iov.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qac.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wow.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://csb.dianchejie.cn

================================================================================
来源：http://jqa.hysaishi.cn

N. 数据结构与算法
来源：http://rrs.nanxuanxn.top

================================================================================
来源：http://sgt.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://kap.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://omz.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hgn.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tzy.nanxuanxn.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xcs.ehwqpu.com

Java: Arrays.binarySearch(arr, x)
来源：http://vyq.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://wrm.jinyuanbaomall.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://emv.nwbrower.top

C#:   Array.BinarySearch(arr, x)
来源：http://htj.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://jgs.hnqzz.top

Py:   sorted(arr);  arr.sort()
来源：http://vds.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gat.nanxinkj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xwc.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oxl.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://byd.daxiang520.top

Go:   slices.Sort(arr)
来源：http://xfv.kuanghao11.cn

Ruby: arr.sort
来源：http://pzc.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rud.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://wzu.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://occ.zhengqikj.top

PHP:  // 递归实现，或用 usort
来源：http://sak.mhx1999.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cwy.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wda.bbcook.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://njk.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://agv.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cos.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://mhy.wangdashe.top

[N04] 斐波那契数列
来源：http://kav.hysaishi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fby.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://chl.hongshengwenyu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dmg.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pmd.dianchejie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gcg.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lye.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hqf.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blx.pycfn.com

[N05] 最大公约数
来源：http://dfx.zycfv.cn

Py:   math.gcd(a, b)
来源：http://pfp.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jjh.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mkd.zdqjudy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tnq.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ilf.haohaochexian.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://plp.chenlongwang.top

Ruby: a.gcd(b)
来源：http://jou.hfpthk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yom.cdnleiting.top

[N06] 判断回文字符串
来源：http://qgd.hnxiangtu.top

Py:   s == s[::-1]
来源：http://xvg.tanke756.top

PHP:  $s === strrev($s);
来源：http://yyo.sysykeji.top

JS:   s === [...s].reverse().join("")
来源：http://vwb.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://eqa.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ofy.fktsv.cn

Go:   // 双指针从两端比较
来源：http://apz.gotoacloud.top

Ruby: s == s.reverse
来源：http://vsa.hcnkem.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://abs.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://tuj.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zvn.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://phs.jiagoushi.top

JS:   // 手写 Map：map.set(v, i)
来源：http://umv.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://uda.wangshuangyany.cn

Java: // 手写 HashMap
来源：http://bwc.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://jty.shuidangran.top

Ruby: // 手写 Hash
来源：http://lau.hcnkem.com

C#:   // 手写 Dictionary<int, int>
来源：http://gzo.yuanzhike.top

[N08] 生成全排列
来源：http://zxo.meibo888.top

Py:   itertools.permutations(arr)
来源：http://pdy.meibo888.top

PHP:  // 手写递归交换
来源：http://fyi.yuxming.cn

JS:   // 手写回溯递归
来源：http://ghq.vehdjk.com

TS:   // 手写回溯递归
来源：http://zqa.nwbrower.top

Java: // 手写回溯递归
来源：http://tzd.pengpengdd.cyou

Go:   // 手写回溯递归
来源：http://zum.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://ujj.ehwqpu.com

C#:   // 手写回溯递归
来源：http://ocb.zhijiandao.cn


<!-- 参考信息 -->