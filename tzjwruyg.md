代发 wailian999

================================================================================
来源：http://msh.gzhubu.top

K. JSON 与序列化
来源：http://bci.shangyingyoupin.top

================================================================================
来源：http://qzp.hnxiangtu.top

[K01] 对象转 JSON 字符串
来源：http://bvt.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jgu.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jip.cashguo.top

JS:   JSON.stringify(obj)
来源：http://mjp.shzxlz.cn

TS:   JSON.stringify(obj)
来源：http://unt.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://svq.jianghu66.top

Go:   json.Marshal(obj)
来源：http://uis.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://exb.jqgfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://eii.yj202588.top

[K02] JSON 字符串转对象
来源：http://tsu.shuidangran.top

Py:   json.loads(s)
来源：http://lwx.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uuk.cucudq.cn

JS:   JSON.parse(s)
来源：http://qcv.epnwcf.com

TS:   JSON.parse(s)
来源：http://orp.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pgp.fengsongda.top

Go:   json.Unmarshal(data, &v)
来源：http://ejx.redwolf501.top

Ruby: JSON.parse(s)
来源：http://aii.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://piz.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://mgd.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nxb.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iwo.yuanzhike.top

JS:   JSON.stringify(obj, null, 2)
来源：http://efe.ivvv.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sex.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ebg.guannengcc.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yqf.ppjwa.cn

Ruby: JSON.pretty_generate(obj)
来源：http://znq.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ncs.fzhhl.top

[K04] 读取 JSON 文件
来源：http://pfk.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dzh.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tgw.316326.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qiv.hnqzz.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yhf.ybcxt.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cas.fengsongda.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gvf.dianchejie.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ftt.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kfm.hesvh.cn

[K05] 深拷贝对象
来源：http://hrc.yongpay.top

Py:   copy.deepcopy(obj)
来源：http://bds.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://bko.guannengcc.top

JS:   structuredClone(obj)
来源：http://iyf.svipenyu.cn

TS:   structuredClone(obj)
来源：http://xpb.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ues.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hfn.fanxiaobao.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rxp.tarul.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mgl.uphjek.com

[K06] 解析 URL 查询串
来源：http://irc.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dhy.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xvm.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gjl.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rtr.9152youxi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blp.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jon.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dtk.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ngb.yfazqb.com

[K07] 进制转换
来源：http://qnr.sjlbkw.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yuv.smart0.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pmp.vehdjk.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lhv.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qmk.ywan-chungtsiang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gvj.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://srk.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ilh.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fgn.sxryk.cn

[K08] 二进制序列化（非 JSON）
来源：http://rmq.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://fkf.c1oappe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lcp.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://gig.tian-w.cn

TS:   v8.serialize(obj)        // Node
来源：http://dbv.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vwj.haohaochexian.top

Go:   encoding/gob
来源：http://dpn.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://rwx.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://boa.zhijiandao.cn

================================================================================
来源：http://nre.bjfxy.top

L. 网络请求
来源：http://pnd.yuxming.cn

================================================================================
来源：http://blq.yueranfly.top

[L01] 发送 GET 请求
来源：http://lmn.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kti.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qjj.xinyue.icu

JS:   await fetch(url)
来源：http://cfc.aizwys.cn

TS:   await fetch(url)
来源：http://aoi.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://chk.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://kpf.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://iga.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mhn.zdbjq.cn

[L02] 发送 POST JSON
来源：http://aip.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://vex.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xvh.hongshengwenyu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xci.ydjk.org.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tjy.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://znx.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xie.haohaochexian.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nmi.yfazqb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vop.gzhubu.top

[L03] 设置自定义请求头
来源：http://vmw.ybcxt.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kfg.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://alw.snrcjt.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mbc.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gkk.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jyt.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qwe.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aea.sysykeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mmf.c1oappe.top

[L04] 设置超时
来源：http://ftq.yongpay.top

Py:   requests.get(url, timeout=5)
来源：http://frd.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fif.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gul.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kea.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kba.zhiwuduotai.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dvs.xziqi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qqi.daxiang520.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://upo.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://fdd.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vet.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vil.gaohongyu789.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wei.fehbvm.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cht.andypj.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wov.xziqi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://erh.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nck.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hsx.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://oxc.hongshengwenyu.top

Py:   resp.json()
来源：http://bch.hnqzz.top

PHP:  json_decode($body, true);
来源：http://vbo.zhongyouzk.top

JS:   await resp.json()
来源：http://bpp.hfpthk.cn

TS:   await resp.json()
来源：http://mhk.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zsn.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tuf.guowangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://htg.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cfn.hammf.cn

[L07] 处理 HTTP 状态码
来源：http://zpq.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hlo.gzhubu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fsz.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://ysb.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://drx.tianlin.xyz

Java: resp.statusCode()
来源：http://wmq.hnqzz.top

Go:   resp.StatusCode
来源：http://lja.chenjidiqi.icu

Ruby: resp.code.to_i
来源：http://otx.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://tow.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://lml.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://klx.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://xlh.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://otl.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gfe.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ynj.sxryk.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kwp.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pot.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uzm.hcnkem.com

================================================================================
来源：http://owo.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://zle.wangshuangyany.cn

================================================================================
来源：http://tku.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://wgh.shanyushiyangkeji.top

Py:   sys.argv[1:]
来源：http://gay.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://uqm.yanxiufei.cn

JS:   process.argv.slice(2)
来源：http://jxc.zdbjq.cn

TS:   process.argv.slice(2)
来源：http://srt.meibo888.top

Java: args 数组（main 方法参数）
来源：http://wtj.gaohongyu789.top

Go:   os.Args[1:]
来源：http://bva.zhaomingkeji.xyz

Ruby: ARGV
来源：http://ydq.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://acr.shangyingyoupin.top

[M02] 读取环境变量
来源：http://gfc.hammf.cn

Py:   os.environ.get("HOME")
来源：http://zue.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qgq.nwbrower.top

JS:   process.env.HOME
来源：http://rpd.aibaodan.cn

TS:   process.env.HOME
来源：http://des.fehbvm.com

Java: System.getenv("HOME")
来源：http://dts.hnxiangtu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vif.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://ziu.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fvl.daria6918.cn

[M03] 执行外部命令
来源：http://ryn.fzhhl.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ars.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vey.fzhhl.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zpp.jiagoushi.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nbo.tianlin.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nkt.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gdy.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://mvu.ybcxt.top

C#:   Process.Start("ls", "-l");
来源：http://kua.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://wmc.wangshuangyany.cn

Py:   os.getcwd()
来源：http://cre.shanyushiyangtech.top

PHP:  getcwd();
来源：http://zbz.iojbl.cn

JS:   process.cwd()
来源：http://xrv.yj20258888.top

TS:   process.cwd()
来源：http://oah.guannengcc.top

Java: Path.of("").toAbsolutePath()
来源：http://yyb.xziqi.cn

Go:   os.Getwd()
来源：http://xph.sxryk.cn

Ruby: Dir.pwd
来源：http://xys.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zqk.shuidangran.top

[M05] 设置退出码
来源：http://bpv.jinyuanbaomall.cn

Py:   sys.exit(1)
来源：http://sye.dianchejie.cn

PHP:  exit(1);
来源：http://dxt.vqdsnc.cn

JS:   process.exit(1)
来源：http://ful.dashuyun.cn

TS:   process.exit(1)
来源：http://cqn.hcnkem.com

Java: System.exit(1)
来源：http://ghg.zycfv.cn

Go:   os.Exit(1)
来源：http://imz.yuxming.cn

Ruby: exit 1
来源：http://lfc.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lqc.daria6918.cn

[M06] 向标准错误输出
来源：http://dlh.hysaishi.cn

Py:   print("err", file=sys.stderr)
来源：http://ann.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ims.jiagoushi.top

JS:   console.error("err")
来源：http://sej.yuanzhike.top

TS:   console.error("err")
来源：http://ttx.chenjidiqi.icu

Java: System.err.println("err")
来源：http://vif.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mqo.c1oappe.top

Ruby: warn "err"
来源：http://kwf.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://xsq.yuxming.cn

[M07] 判断是否为主入口
来源：http://fal.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://euk.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gem.snrcjt.cn

JS:   require.main === module
来源：http://ldg.jinqigufen.top

TS:   require.main === module
来源：http://bxt.yonumen.top

Java: public static void main(String[] args)
来源：http://nsi.fktsv.cn

Go:   func main()
来源：http://hpd.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yyo.hammf.cn

C#:   static void Main(string[] args)
来源：http://tti.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://uze.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://faz.quarkkingdee.top

PHP:  PHP_OS;  phpversion();
来源：http://qhw.sweek.top

JS:   process.platform;  process.version
来源：http://xkz.guowangkeji.top

TS:   process.platform;  process.version
来源：http://rcq.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yku.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tyk.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qwi.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vny.chenlongwang.top

================================================================================
来源：http://rrp.fanxiaobao.xyz

N. 数据结构与算法
来源：http://etr.cqqwz.cn

================================================================================
来源：http://hmk.nanxuanxn.top

[N01] 二分查找（有序数组）
来源：http://veo.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vck.xylfe.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lud.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oci.nanxuanxn.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ddv.xuanzx.com

Java: Arrays.binarySearch(arr, x)
来源：http://jxl.yonumen.top

Go:   sort.SearchInts(arr, x)
来源：http://uwr.yj20258.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ntk.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://ceg.jinghuilouyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://nuo.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://kyb.pengpengdd.cyou

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dux.kuanghao11.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fza.yuanzhike.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rxk.hnxiangtu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lmn.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://nig.gotoacloud.top

Ruby: arr.sort
来源：http://jlg.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://esk.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://ykq.hesvh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cbc.aibaodan.cn

PHP:  // 递归实现，或用 usort
来源：http://kni.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cgj.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://brj.birdmap.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yng.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lhq.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eno.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://bbn.vqdsnc.cn

[N04] 斐波那契数列
来源：http://qbk.jinyuanbaomall.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://shi.cucudq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oxx.meibo888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pky.tianlin.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://isr.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bzq.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iin.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bbk.haohaochexian.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fgn.gaohongyu789.top

[N05] 最大公约数
来源：http://nez.yj202588.top

Py:   math.gcd(a, b)
来源：http://ihv.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fqa.jqgufenzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ygs.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://itl.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nyg.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lat.ctjpmb.com

Ruby: a.gcd(b)
来源：http://nlr.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fzm.jinqigufen.top

[N06] 判断回文字符串
来源：http://fgt.wangdashe.top

Py:   s == s[::-1]
来源：http://xju.uphjek.com

PHP:  $s === strrev($s);
来源：http://aut.xingfuxueyuan.xyz

JS:   s === [...s].reverse().join("")
来源：http://cub.cdnleiting.top

TS:   s === [...s].reverse().join("")
来源：http://dom.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oib.jlsjyb.cn

Go:   // 双指针从两端比较
来源：http://znk.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://bja.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kmc.sweek.top

[N07] 两数之和（返回下标）
来源：http://qvy.zdqjudy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jmt.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ifq.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wil.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://kuc.mhx1999.top

Java: // 手写 HashMap
来源：http://fbm.c1oappe.top

Go:   // 手写 map[int]int
来源：http://vnr.hammf.cn

Ruby: // 手写 Hash
来源：http://xiv.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bjn.xziqi.cn

[N08] 生成全排列
来源：http://zpd.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://okc.zycfv.cn

PHP:  // 手写递归交换
来源：http://zef.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://xvl.ydzc1.top

TS:   // 手写回溯递归
来源：http://diw.birdmap.top

Java: // 手写回溯递归
来源：http://ufo.gogol.net.cn

Go:   // 手写回溯递归
来源：http://vrb.zhoulong.xyz

Ruby: arr.permutation.to_a
来源：http://hiy.0kj1m.cn

C#:   // 手写回溯递归
来源：http://kns.xingfuxueyuan.xyz


<!-- 参考信息 -->