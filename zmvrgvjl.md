代发 wailian999

C#:   public / protected / private / internal
来源：http://qkj.yj20258.top

[G11] getter / setter
来源：http://stq.zhoulong.xyz

Py:   @property 与 @x.setter
来源：http://qze.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zbf.yfazqb.com

JS:   get name() { return this._name; }
来源：http://gli.shangyingyoupin.top

TS:   get name(): string { return this._name; }
来源：http://nfj.sufxvd.cn

Java: public String getName() { return name; }
来源：http://qey.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xmb.9152youxi.cn

Ruby: attr_accessor :name
来源：http://djj.fengsongda.top

C#:   public string Name { get; set; }
来源：http://uem.vehdjk.com

[G12] 对象转字符串
来源：http://dql.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://gia.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://byp.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://arr.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://dxs.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://luo.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://scz.fzhhl.top

Ruby: def to_s; @name; end
来源：http://uum.guannengcc.top

C#:   public override string ToString() => Name;
来源：http://hle.chenzaomai.com

[G13] 判断对象类型
来源：http://eki.ehwqpu.com

Py:   isinstance(u, User)
来源：http://gmj.vqdsnc.cn

PHP:  $u instanceof User
来源：http://ttu.xuetiantiany.cn

JS:   u instanceof User
来源：http://khx.iojbl.cn

TS:   u instanceof User
来源：http://tnw.tian-w.cn

Java: u instanceof User
来源：http://npf.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://lup.yj20258888.top

Ruby: u.is_a?(User)
来源：http://skk.fehbvm.com

C#:   u is User
来源：http://dat.hnqzz.top

[G14] 数据类 / record
来源：http://lko.guowangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://boo.xuetiantiany.cn

PHP:  // 用 readonly 属性模拟
来源：http://udg.hfpthk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pak.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://qgp.vehdjk.com

Java: record User(String name, int age) {}
来源：http://oof.vqdsnc.cn

Go:   type User struct { Name string; Age int }
来源：http://rdy.gotoacloud.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hpa.dashuyun.cn

C#:   record User(string Name, int Age);
来源：http://uyb.hongshengwenyu.top

[G15] 枚举
来源：http://tms.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qnk.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://gka.smart0.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qmi.cucudq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zlj.yuanzhike.top

Java: enum Color { RED, GREEN }
来源：http://lmb.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kal.snrcjt.cn

Ruby: Color = %i[red green].freeze
来源：http://omz.jqgufenzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fxj.chenjidiqi.icu

[G16] 对象转数组 / 字典
来源：http://diw.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://juf.sxryk.cn

PHP:  get_object_vars($obj);
来源：http://tbi.hywenlv.cn

JS:   Object.entries(obj)
来源：http://khf.cqqwz.cn

TS:   Object.entries(obj)
来源：http://itf.tarul.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://htz.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://otc.yueranfly.top

Ruby: obj.instance_variables
来源：http://yjp.quarkkingdee.top

C#:   // 用反射或 System.Text.Json
来源：http://gvq.c1oappe.top

================================================================================
来源：http://yxh.iojbl.cn

H. 异常与错误处理
来源：http://irb.hysaishi.cn

================================================================================
来源：http://quj.chenzaomai.com

[H01] try / catch 基础
来源：http://kaq.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aub.aizwys.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://alg.havefunace.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://byo.hfpthk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://agi.epnwcf.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pgd.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://siq.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zfl.kuanghao11.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rqv.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://qdy.snrcjt.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kob.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://yat.zdbjq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ydw.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://qct.jlsjyb.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jwi.yangfankeji.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://zpn.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://fet.jinqigufen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://exq.nanxinkj.top

[H03] 主动抛出异常
来源：http://dhd.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://xev.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hhe.xylfe.cn

JS:   throw new Error("错误信息");
来源：http://ryz.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://mwn.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nne.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fcy.vehdjk.com

Ruby: raise ArgumentError, "错误信息"
来源：http://goi.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://afr.tanke756.top

[H04] 自定义异常类型
来源：http://smt.dashuyun.cn

Py:   class MyError(Exception): pass
来源：http://nfc.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://xgo.yj20258.top

JS:   class MyError extends Error {}
来源：http://bdi.jqgfzy.top

TS:   class MyError extends Error {}
来源：http://fad.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://wpa.zhengqikj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wqp.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://bag.hcnkem.com

C#:   class MyException : Exception {}
来源：http://fie.quarkkingdee.top

[H05] 捕获特定类型
来源：http://vlv.shanyushiyangtech.top

Py:   except ValueError as e:
来源：http://wvu.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jkr.nanxuanxn.top

JS:   if (e instanceof TypeError) {}
来源：http://drk.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://xzq.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://qyo.ywan-chungtsiang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zqn.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://lye.vehdjk.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dwq.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://bpd.nanxinkj.top

Py:   value = d.get("k") or default
来源：http://uuq.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://crf.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://efp.ydzc1.top

TS:   obj?.a?.b;  d ?? default
来源：http://zib.jlsjyb.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://avj.svipenyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fal.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://sif.jinqigufen.top

C#:   obj?.A?.B ?? default
来源：http://isk.zhixingplan.top

[H07] 断言
来源：http://qwv.birdmap.top

Py:   assert x > 0, "必须为正"
来源：http://twi.yangfankeji.com

PHP:  assert($x > 0);
来源：http://zmc.svipenyu.cn

JS:   console.assert(x > 0);
来源：http://yjq.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://bod.xingfuxueyuan.xyz

Java: assert x > 0 : "必须为正";
来源：http://vrk.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zpa.yonumen.top

Ruby: raise "必须为正" unless x > 0
来源：http://zgp.jqgufenzy.top

C#:   Debug.Assert(x > 0);
来源：http://kfn.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://jux.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://wak.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kwb.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://egw.yj202588.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lmo.xziqi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://czf.shangyingyoupin.top

Go:   err.Error()
来源：http://loc.jiagoushi.top

Ruby: e.message;  e.backtrace
来源：http://car.jlsjyb.cn

C#:   e.Message;  e.StackTrace
来源：http://zom.guannengcc.top

[H09] 带错误码的异常
来源：http://yoq.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wam.hywenlv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mru.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kyd.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hrq.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sjc.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mig.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://plv.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://gzl.yvedp.cn

[H10] 资源自动释放
来源：http://hsg.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sqv.svipenyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zoi.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tbj.bbcook.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pme.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kll.svipenyu.cn

Go:   defer f.Close()
来源：http://vwy.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ger.yanxiufei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hxc.0kj1m.cn

================================================================================
来源：http://nfw.ehwqpu.com

I. 正则表达式
来源：http://dto.ydzc1.top

================================================================================
来源：http://jld.hcnkem.com

[I01] 判断是否匹配
来源：http://zuc.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jjp.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://rsu.xuetiantiany.cn

JS:   /\d+/.test(s)
来源：http://bec.yj20258.top

TS:   /\d+/.test(s)
来源：http://lki.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uek.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dyg.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://kbz.ydzc1.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://suh.chenzaomai.com

[I02] 提取所有匹配
来源：http://alc.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://mtb.yj202588.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://glw.pycfn.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vvj.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://xke.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dap.cashguo.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nrm.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://qyd.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://evo.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://uhh.tanke756.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jkg.yj20258888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pcl.aibaodan.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lut.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qgi.kuanghao11.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ddf.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bec.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ngo.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jwr.jqgufenzy.top

[I04] 正则替换
来源：http://eyn.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://lfr.yuanzhike.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gke.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://fui.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://vxr.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://efc.jlsjyb.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ihu.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://dkn.havefunace.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://abf.cashguo.top

[I05] 按正则拆分
来源：http://gqr.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nsw.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dde.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://chx.cashguo.top

TS:   s.split(/\s*,\s*/)
来源：http://con.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://fvc.ppjwa.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lzs.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ipw.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jsm.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cyu.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hpa.hongshengwenyu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aev.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wqg.dashuyun.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://alb.jlsjyb.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tvl.xylfe.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fap.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ttr.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pfs.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://nkn.yangfankeji.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://grf.nanxuanxn.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wxl.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qkt.shanyushiyangtech.top

TS:   /error/gim
来源：http://pij.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://apb.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iyn.zhoulong.xyz

Ruby: s.scan(/error/i)
来源：http://pza.kuanghao11.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://piz.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://wnl.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://smu.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://asj.sxryk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ppi.zycfv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sry.chenlongwang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ofd.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qws.fanxiaobao.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yxw.dashuyun.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eey.jqgfzy.top

================================================================================
来源：http://aym.iojbl.cn

J. 日期与时间
来源：http://wak.0kj1m.cn

================================================================================
来源：http://fss.zdqjudy.top

[J01] 获取当前时间
来源：http://yqp.iojbl.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://phm.gotoacloud.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dqg.c1oappe.top

JS:   new Date();  Date.now()
来源：http://fyk.shuidangran.top

TS:   new Date();  Date.now()
来源：http://rhj.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://iiq.chenlongwang.top

Go:   time.Now()
来源：http://dbj.c1oappe.top

Ruby: Time.now
来源：http://arc.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xva.dianchejie.cn

[J02] 格式化输出
来源：http://hfu.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hqe.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wyt.guowangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cad.gotoacloud.top

TS:   d.toISOString()
来源：http://kbl.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://axv.jiagoushi.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nqw.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wan.ydjk.org.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rle.jinqigufen.top

[J03] 字符串解析为日期
来源：http://tyq.kuanghao11.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eqv.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gaq.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://qfy.ctjpmb.com

TS:   new Date("2024-01-02")
来源：http://wkz.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://vgr.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://phs.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://gwb.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://okk.vehdjk.com

[J04] 时间戳与日期互转
来源：http://rdr.hcnkem.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fdo.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ggn.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ibb.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sol.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rrd.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bib.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tzc.zhoulong.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ukt.hcnkem.com

[J05] 时间加减（加 7 天）
来源：http://ply.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://mtm.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pnr.hesvh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pwh.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uey.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://lhw.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qmv.c1oappe.top

Ruby: Time.now + 7 * 86400
来源：http://hcv.jqgufenzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://nrz.xinyue.icu

[J06] 计算两时间之差
来源：http://xuu.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://lqr.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://vna.xinyue.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://keq.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cgx.pengpengdd.cyou

Java: Duration.between(start, end).toSeconds()
来源：http://uyg.mhx1999.top

Go:   end.Sub(start).Hours()
来源：http://xml.sufxvd.cn

Ruby: end - start                 # 返回秒数
来源：http://ulb.sysykeji.top

C#:   (end - start).TotalSeconds
来源：http://ham.epnwcf.com

[J07] 比较两个日期
来源：http://oov.epnwcf.com

Py:   d1 < d2;  d1 == d2
来源：http://art.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aqm.yj20258888.top

JS:   d1.getTime() < d2.getTime()
来源：http://dqx.andypj.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://cpr.cucudq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ags.9152youxi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wwd.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://shc.chenjidiqi.icu

C#:   d1 < d2;  d1 == d2
来源：http://cgc.hnqzz.top

[J08] 提取年月日与星期
来源：http://ppo.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wll.bjfxy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pnc.kuanghao11.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://feq.xinyue.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://afy.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gjg.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sbi.pycfn.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vle.fehbvm.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bil.xziqi.cn

[J09] 时区处理
来源：http://ukg.yj20258.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sci.dianchejie.cn


<!-- 参考信息 -->