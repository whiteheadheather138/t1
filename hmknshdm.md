代发 wailian999

================================================================================
来源：http://asm.xuanzx.com

K. JSON 与序列化
来源：http://kbn.jqgufenzy.top

================================================================================
来源：http://pup.mhx1999.top

[K01] 对象转 JSON 字符串
来源：http://mll.yueranfly.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mbn.tianlin.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://brm.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://fpo.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://lkn.xingfuxueyuan.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dnj.zdqjudy.top

Go:   json.Marshal(obj)
来源：http://yfp.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://gja.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://stc.ybcxt.top

[K02] JSON 字符串转对象
来源：http://upp.fanxiaobao.xyz

Py:   json.loads(s)
来源：http://pft.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jlw.tianlin.xyz

JS:   JSON.parse(s)
来源：http://gqi.svipenyu.cn

TS:   JSON.parse(s)
来源：http://lef.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bhv.fzhhl.top

Go:   json.Unmarshal(data, &v)
来源：http://nvn.jlsjyb.cn

Ruby: JSON.parse(s)
来源：http://znv.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://reb.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://zko.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gox.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vrm.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://abe.aibaodan.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vsx.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jmd.sxryk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gol.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xoa.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dps.yuanzhike.top

[K04] 读取 JSON 文件
来源：http://xys.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tan.jianghu66.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tcd.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wrt.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xxi.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zlc.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gex.chenzaomai.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://lce.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wty.guowangkeji.top

[K05] 深拷贝对象
来源：http://rnw.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://mcl.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://tub.52xcode.cn

JS:   structuredClone(obj)
来源：http://whs.yongpay.top

TS:   structuredClone(obj)
来源：http://vjq.jqgufenzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://btn.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tip.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://edx.zdbjq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qke.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://gev.zhongyouzk.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bae.hammf.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://aku.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mgs.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fmw.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://eqj.zhaomingkeji.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://kzs.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://egc.hfpthk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ugl.bjfxy.top

[K07] 进制转换
来源：http://ydq.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zxw.tian-w.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jkj.c1oappe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oqb.yuxming.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://frl.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iam.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xgm.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wkp.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wuj.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://dkl.pycfn.com

Py:   pickle.dumps(obj)
来源：http://fjj.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://kcl.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://ptv.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://acd.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fag.zhijiandao.cn

Go:   encoding/gob
来源：http://wtw.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://jzm.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tuv.yvedp.cn

================================================================================
来源：http://whm.cashguo.top

L. 网络请求
来源：http://qem.yuxming.cn

================================================================================
来源：http://ngg.yj20258.top

[L01] 发送 GET 请求
来源：http://snd.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xuc.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zbg.zdqjudy.top

JS:   await fetch(url)
来源：http://txv.yuanzhike.top

TS:   await fetch(url)
来源：http://ibr.sxryk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oao.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://fjt.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kvj.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jom.cucudq.cn

[L02] 发送 POST JSON
来源：http://fdk.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wkj.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yqp.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tee.zhiwuduotai.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xnz.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gir.c1oappe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ims.sjlbkw.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rdk.birdmap.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://boh.bjfxy.top

[L03] 设置自定义请求头
来源：http://nrs.zdqjudy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mlp.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ouw.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qdy.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kbk.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bbx.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vqu.xinyue.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wsr.aizwys.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pbg.yfazqb.com

[L04] 设置超时
来源：http://jtx.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://zxb.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wzq.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aki.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dcy.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mhw.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oqh.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gfs.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mvg.epnwcf.com

[L05] 上传文件（multipart）
来源：http://uvx.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pkd.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://auq.gzhubu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://feh.zhiwuduotai.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pxg.jinqigufen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ajj.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://srh.c1oappe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qgk.hnqzz.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://foa.smart0.xyz

[L06] 解析响应为 JSON
来源：http://qbt.ehwqpu.com

Py:   resp.json()
来源：http://fwn.xziqi.cn

PHP:  json_decode($body, true);
来源：http://exy.316326.xyz

JS:   await resp.json()
来源：http://ntx.epnwcf.com

TS:   await resp.json()
来源：http://puq.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nyu.ybcxt.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://otw.fengsongda.top

Ruby: JSON.parse(resp.body)
来源：http://bff.hnqzz.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jrh.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://uqv.ppjwa.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://obd.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://utx.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://ujj.shanyushiyangkeji.top

TS:   resp.ok;  resp.status
来源：http://yym.zdbjq.cn

Java: resp.statusCode()
来源：http://hos.jiagoushi.top

Go:   resp.StatusCode
来源：http://yrx.hysaishi.cn

Ruby: resp.code.to_i
来源：http://zzi.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://uep.tarul.cn

[L08] 并发请求多个地址
来源：http://guh.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://whz.guowangkeji.top

PHP:  curl_multi_init() 系列
来源：http://xit.pycfn.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://czb.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qnw.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mxz.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cxw.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jjt.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://huh.guowangkeji.top

================================================================================
来源：http://cqn.zdbjq.cn

M. 命令行 / 进程 / 环境
来源：http://fig.ctjpmb.com

================================================================================
来源：http://gii.jlsjyb.cn

[M01] 读取命令行参数
来源：http://iij.ivvv.top

Py:   sys.argv[1:]
来源：http://auj.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://pmv.zdqjudy.top

JS:   process.argv.slice(2)
来源：http://fyl.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://yqx.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://ooz.yj20258.top

Go:   os.Args[1:]
来源：http://fds.hesvh.cn

Ruby: ARGV
来源：http://psw.cdnleiting.top

C#:   args 数组（Main 方法参数）
来源：http://yho.gotoacloud.top

[M02] 读取环境变量
来源：http://cxh.aizwys.cn

Py:   os.environ.get("HOME")
来源：http://suo.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rec.zdbjq.cn

JS:   process.env.HOME
来源：http://sch.hcnkem.com

TS:   process.env.HOME
来源：http://eih.jinqigufen.top

Java: System.getenv("HOME")
来源：http://mlj.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jda.shuidangran.top

Ruby: ENV["HOME"]
来源：http://rre.hnxiangtu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://duk.jyoumei.cn

[M03] 执行外部命令
来源：http://nht.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rbq.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wxo.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zan.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lmt.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://val.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://wat.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zub.cqqwz.cn

C#:   Process.Start("ls", "-l");
来源：http://jks.ybcxt.top

[M04] 获取当前工作目录
来源：http://swe.quarkkingdee.top

Py:   os.getcwd()
来源：http://ivg.hysaishi.cn

PHP:  getcwd();
来源：http://mji.jqgfzy.top

JS:   process.cwd()
来源：http://stp.tian-w.cn

TS:   process.cwd()
来源：http://chi.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://rou.shzxlz.cn

Go:   os.Getwd()
来源：http://kuy.birdmap.top

Ruby: Dir.pwd
来源：http://cws.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://awv.jiagoushi.top

[M05] 设置退出码
来源：http://fev.jinghuilouyu.cn

Py:   sys.exit(1)
来源：http://dey.tian-w.cn

PHP:  exit(1);
来源：http://hck.wangshuangyany.cn

JS:   process.exit(1)
来源：http://alj.shangyingyoupin.top

TS:   process.exit(1)
来源：http://mct.hnqzz.top

Java: System.exit(1)
来源：http://ygx.yuxming.cn

Go:   os.Exit(1)
来源：http://qmk.feifeiyinyue.top

Ruby: exit 1
来源：http://ckc.zhiwuduotai.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vop.zhongyouzk.top

[M06] 向标准错误输出
来源：http://szp.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://aen.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kui.c1oappe.top

JS:   console.error("err")
来源：http://eyr.nwbrower.top

TS:   console.error("err")
来源：http://iyl.wangdashe.top

Java: System.err.println("err")
来源：http://ela.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tvf.yuxming.cn

Ruby: warn "err"
来源：http://lga.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://jpe.jinqigufen.top

[M07] 判断是否为主入口
来源：http://czo.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://kew.shanyushiyangtech.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bzn.yuxming.cn

JS:   require.main === module
来源：http://kmq.zhijiandao.cn

TS:   require.main === module
来源：http://kov.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://nwn.sysykeji.top

Go:   func main()
来源：http://jro.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://siu.jinghuilouyu.cn

C#:   static void Main(string[] args)
来源：http://zil.svipenyu.cn

[M08] 获取系统与运行时信息
来源：http://weq.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://bqd.ydjk.org.cn

PHP:  PHP_OS;  phpversion();
来源：http://hhj.jinqigufen.top

JS:   process.platform;  process.version
来源：http://kfq.epnwcf.com

TS:   process.platform;  process.version
来源：http://fql.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vrw.meibo888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zfr.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kct.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dtg.jqgfzy.top

================================================================================
来源：http://maw.hnxiangtu.top

N. 数据结构与算法
来源：http://bxq.pycfn.com

================================================================================
来源：http://oxy.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://jdy.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://saz.hnqzz.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dji.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ddn.iojbl.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://adc.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://pvi.ctjpmb.com

Go:   sort.SearchInts(arr, x)
来源：http://vrg.hfpthk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mdo.xylfe.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ynq.guowangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://nxi.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://inn.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qgd.c1oappe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kym.birdmap.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xqp.ehwqpu.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pfo.yuxming.cn

Go:   slices.Sort(arr)
来源：http://zwl.xziqi.cn

Ruby: arr.sort
来源：http://ddl.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hwm.bjfxy.top

[N03] 快速排序（分治示例）
来源：http://rtn.jinyuanbaomall.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bjo.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://dlz.bbcook.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ipy.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://neh.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kwa.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cqk.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qcu.xingfuxueyuan.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://esn.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://ptz.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fua.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://toc.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sxq.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hpe.xziqi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tbx.fzhhl.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ksx.zdqjudy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nht.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qrz.yvedp.cn

[N05] 最大公约数
来源：http://bxa.xingfuxueyuan.xyz

Py:   math.gcd(a, b)
来源：http://jqx.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wrb.fengsongda.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cxi.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mgy.zhiwuduotai.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ftr.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cnn.ivvv.top

Ruby: a.gcd(b)
来源：http://nvf.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jsd.haohaochexian.top

[N06] 判断回文字符串
来源：http://vcq.xuanzx.com

Py:   s == s[::-1]
来源：http://jpv.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://vpv.sxryk.cn

JS:   s === [...s].reverse().join("")
来源：http://yyi.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://ubu.zhiwuduotai.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rih.zhongyouzk.top

Go:   // 双指针从两端比较
来源：http://yhb.jiagoushi.top

Ruby: s == s.reverse
来源：http://num.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cwc.feifeiyinyue.top

[N07] 两数之和（返回下标）
来源：http://iai.hammf.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ngt.zycfv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ndb.nanxinkj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nry.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://lun.yuanzhike.top

Java: // 手写 HashMap
来源：http://ltm.gaohongyu789.top

Go:   // 手写 map[int]int
来源：http://vzu.vehdjk.com

Ruby: // 手写 Hash
来源：http://qeb.sufxvd.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vtc.haohaochexian.top

[N08] 生成全排列
来源：http://jlo.yuanzhike.top

Py:   itertools.permutations(arr)
来源：http://jvt.jiagoushi.top

PHP:  // 手写递归交换
来源：http://lcw.daxiang520.top

JS:   // 手写回溯递归
来源：http://lzp.hammf.cn

TS:   // 手写回溯递归
来源：http://wsl.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://iez.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://lcb.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://jtp.ctjpmb.com

C#:   // 手写回溯递归
来源：http://wqc.shzxlz.cn


<!-- 参考信息 -->