代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hci.daria6918.cn

Go:   json.Marshal(obj)
来源：http://lyd.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uia.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kcw.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://uwt.shangyingyoupin.top

Py:   json.loads(s)
来源：http://mss.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oim.yongpay.top

JS:   JSON.parse(s)
来源：http://oki.quarkkingdee.top

TS:   JSON.parse(s)
来源：http://cia.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://inn.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://zxo.sysykeji.top

Ruby: JSON.parse(s)
来源：http://oss.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://khc.nanxuanxn.top

[K03] JSON 美化输出（带缩进）
来源：http://udw.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rxs.redwolf501.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rtr.redwolf501.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bxk.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cqf.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ldt.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kkd.yuanzhike.top

Ruby: JSON.pretty_generate(obj)
来源：http://ctb.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lxe.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://ghu.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sro.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://epl.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://whl.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fba.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uvy.zdbjq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lzw.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://vfv.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zon.zdqjudy.top

[K05] 深拷贝对象
来源：http://aed.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://blb.jlsjyb.cn

PHP:  unserialize(serialize($obj));
来源：http://yds.havefunace.top

JS:   structuredClone(obj)
来源：http://hxw.daxiang520.top

TS:   structuredClone(obj)
来源：http://min.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xcy.yvedp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wwa.vqdsnc.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://epb.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hbb.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://plp.yanxiufei.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://guz.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pau.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://enl.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yob.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dsg.sysykeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lek.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mmt.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fcg.yj202588.top

[K07] 进制转换
来源：http://snh.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://grr.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zly.yj20258.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qcp.zhijiandao.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mvf.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sir.yvedp.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rfb.chenzaomai.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://znm.ppjwa.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gyf.jinghuilouyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://llo.quarkkingdee.top

Py:   pickle.dumps(obj)
来源：http://ycc.nanxinkj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://civ.gogol.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://ymi.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://jup.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kuq.guannengcc.top

Go:   encoding/gob
来源：http://pdt.yanxiufei.cn

Ruby: Marshal.dump(obj)
来源：http://sib.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iqq.nanxinkj.top

================================================================================
来源：http://wao.guannengcc.top

L. 网络请求
来源：http://tas.yfazqb.com

================================================================================
来源：http://ubo.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://wom.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kpl.dianchejie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ceo.tanke756.top

JS:   await fetch(url)
来源：http://ufb.zhaomingkeji.xyz

TS:   await fetch(url)
来源：http://gle.52xcode.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kko.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://heg.tarul.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://faj.shuidangran.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mre.uphjek.com

[L02] 发送 POST JSON
来源：http://cwx.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bja.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wju.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bil.jinyuanbaomall.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://smk.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qmi.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lqy.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ofg.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xjb.nwbrower.top

[L03] 设置自定义请求头
来源：http://nqg.xingfuxueyuan.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jkj.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ewh.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wky.kuanghao11.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://slq.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ijd.yueranfly.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hlz.dianchejie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jyx.yonumen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://txi.hongshengwenyu.top

[L04] 设置超时
来源：http://iks.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://gzx.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mkm.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ltx.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ned.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dvc.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xje.tian-w.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gjw.hnqzz.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pnw.c1oappe.top

[L05] 上传文件（multipart）
来源：http://ukd.meibo888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jdz.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://trt.uphjek.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iyo.jianghu66.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ran.tianlin.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jyd.xylfe.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ilt.yuanzhike.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://myx.guannengcc.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hdu.bbcook.cn

[L06] 解析响应为 JSON
来源：http://pep.shangyingyoupin.top

Py:   resp.json()
来源：http://zpj.havefunace.top

PHP:  json_decode($body, true);
来源：http://zxq.316326.xyz

JS:   await resp.json()
来源：http://yei.hywenlv.cn

TS:   await resp.json()
来源：http://pun.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vgq.jinqigufen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dpw.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://ohy.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ovi.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://jfb.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dye.nanxuanxn.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pua.jlsjyb.cn

JS:   resp.ok;  resp.status
来源：http://ome.zhixingplan.top

TS:   resp.ok;  resp.status
来源：http://mju.ctjpmb.com

Java: resp.statusCode()
来源：http://jzx.ivvv.top

Go:   resp.StatusCode
来源：http://spu.9152youxi.cn

Ruby: resp.code.to_i
来源：http://kgl.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://owf.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://bme.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pmd.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://hdp.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mue.sysykeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ohm.gzhubu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://beo.jlsjyb.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nsl.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fgq.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tmc.xuetiantiany.cn

================================================================================
来源：http://yjf.bjfxy.top

M. 命令行 / 进程 / 环境
来源：http://nsi.fzhhl.top

================================================================================
来源：http://lgi.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://npn.jlsjyb.cn

Py:   sys.argv[1:]
来源：http://cel.hfpthk.cn

PHP:  $argv;  $argc;
来源：http://baa.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://uyw.jinqigufen.top

TS:   process.argv.slice(2)
来源：http://lrp.jinghuilouyu.cn

Java: args 数组（main 方法参数）
来源：http://xop.yangfankeji.com

Go:   os.Args[1:]
来源：http://ejt.meibo888.top

Ruby: ARGV
来源：http://vrl.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://nfr.jiagoushi.top

[M02] 读取环境变量
来源：http://vlw.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://abp.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://okp.cucudq.cn

JS:   process.env.HOME
来源：http://jjk.sxryk.cn

TS:   process.env.HOME
来源：http://moq.fzhhl.top

Java: System.getenv("HOME")
来源：http://alk.sysykeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oov.zycfv.cn

Ruby: ENV["HOME"]
来源：http://rkk.pengpengdd.cyou

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yyq.zhoulong.xyz

[M03] 执行外部命令
来源：http://poo.fzhhl.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vik.shanyushiyangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://byn.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://cwi.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bid.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gtb.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ofo.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://dsv.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://ria.yonumen.top

[M04] 获取当前工作目录
来源：http://czs.cheryme.top

Py:   os.getcwd()
来源：http://auj.xziqi.cn

PHP:  getcwd();
来源：http://ysr.ydjk.org.cn

JS:   process.cwd()
来源：http://wwq.wangshuangyany.cn

TS:   process.cwd()
来源：http://rks.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://xbi.xziqi.cn

Go:   os.Getwd()
来源：http://ipr.daria6918.cn

Ruby: Dir.pwd
来源：http://gvw.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://zqf.hysaishi.cn

[M05] 设置退出码
来源：http://qul.snrcjt.cn

Py:   sys.exit(1)
来源：http://eno.andypj.xyz

PHP:  exit(1);
来源：http://bbi.gotoacloud.top

JS:   process.exit(1)
来源：http://tve.dianchejie.cn

TS:   process.exit(1)
来源：http://nal.ybcxt.top

Java: System.exit(1)
来源：http://tys.cdnleiting.top

Go:   os.Exit(1)
来源：http://cch.ydzc1.top

Ruby: exit 1
来源：http://xwi.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bxd.sxryk.cn

[M06] 向标准错误输出
来源：http://ven.52xcode.cn

Py:   print("err", file=sys.stderr)
来源：http://bkc.fanxiaobao.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://dfu.hongshengwenyu.top

JS:   console.error("err")
来源：http://wrh.zhaomingkeji.xyz

TS:   console.error("err")
来源：http://coi.fengsongda.top

Java: System.err.println("err")
来源：http://ieh.wangshuangyany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tgw.mhx1999.top

Ruby: warn "err"
来源：http://bvd.fehbvm.com

C#:   Console.Error.WriteLine("err")
来源：http://nim.wangdashe.top

[M07] 判断是否为主入口
来源：http://pnw.haohaochexian.top

Py:   if __name__ == "__main__":
来源：http://muj.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ozl.birdmap.top

JS:   require.main === module
来源：http://mvw.hcnkem.com

TS:   require.main === module
来源：http://tgy.daria6918.cn

Java: public static void main(String[] args)
来源：http://lgr.xingfuxueyuan.xyz

Go:   func main()
来源：http://hts.sweek.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gpm.daria6918.cn

C#:   static void Main(string[] args)
来源：http://ado.shzxlz.cn

[M08] 获取系统与运行时信息
来源：http://eeu.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://rik.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://dnj.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://hse.epnwcf.com

TS:   process.platform;  process.version
来源：http://luh.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://peb.cqqwz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vxh.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rcc.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://nen.316326.xyz

================================================================================
来源：http://mbl.zhengqikj.top

N. 数据结构与算法
来源：http://iyn.aibaodan.cn

================================================================================
来源：http://kxx.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://yvp.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://dfk.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mwq.ywan-chungtsiang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ghl.nanxuanxn.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://utu.316326.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://lky.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://fag.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://cmc.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://lkx.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://mfc.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://ptg.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vkd.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dhq.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qcy.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jee.chenzaomai.com

Go:   slices.Sort(arr)
来源：http://wfn.tarul.cn

Ruby: arr.sort
来源：http://cwm.sweek.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://evh.shangyingyoupin.top

[N03] 快速排序（分治示例）
来源：http://vcu.smart0.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nlt.iojbl.cn

PHP:  // 递归实现，或用 usort
来源：http://bvk.nwbrower.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jzw.mhx1999.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ena.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://smw.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aad.xylfe.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dyv.shzxlz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://glj.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://dzi.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cnj.nwbrower.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mmd.xinyue.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fqy.yvedp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zdd.gzhubu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pbo.fanxiaobao.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tux.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fym.redwolf501.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jte.zhijiandao.cn

[N05] 最大公约数
来源：http://xoh.zhijiandao.cn

Py:   math.gcd(a, b)
来源：http://nnp.hnqzz.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jmi.shuidangran.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bbe.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dvb.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pro.fanxiaobao.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ixu.hywenlv.cn

Ruby: a.gcd(b)
来源：http://cqi.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ohz.dashuyun.cn

[N06] 判断回文字符串
来源：http://vcl.sufxvd.cn

Py:   s == s[::-1]
来源：http://rpn.ydzc1.top

PHP:  $s === strrev($s);
来源：http://xvp.cdnleiting.top

JS:   s === [...s].reverse().join("")
来源：http://shk.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://owd.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lcu.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://rpr.zhiwuduotai.top

Ruby: s == s.reverse
来源：http://dub.chenlongwang.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vay.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://jah.zhongyouzk.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ogg.tanke756.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ldo.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yxj.sysykeji.top

TS:   // 手写 Map<string, number>
来源：http://auc.hnqzz.top

Java: // 手写 HashMap
来源：http://zwq.havefunace.top

Go:   // 手写 map[int]int
来源：http://goi.xuanzx.com

Ruby: // 手写 Hash
来源：http://ocm.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://trs.zhengqikj.top

[N08] 生成全排列
来源：http://nza.sjlbkw.cn

Py:   itertools.permutations(arr)
来源：http://hlj.hcnkem.com

PHP:  // 手写递归交换
来源：http://jbm.hcnkem.com

JS:   // 手写回溯递归
来源：http://jwv.hywenlv.cn

TS:   // 手写回溯递归
来源：http://mng.hfpthk.cn

Java: // 手写回溯递归
来源：http://fvx.fanxiaobao.xyz

Go:   // 手写回溯递归
来源：http://wfj.aizwys.cn

Ruby: arr.permutation.to_a
来源：http://wkr.shanyushiyangtech.top

C#:   // 手写回溯递归
来源：http://eew.gotoacloud.top

[N09] 栈与队列
来源：http://rrh.jyoumei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bqi.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ewy.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://czs.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hir.yuanzhike.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xdx.hnxiangtu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ifh.52xcode.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wms.cucudq.cn


<!-- 参考信息 -->