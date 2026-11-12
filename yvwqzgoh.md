代发 wailian999

JS:   get name() { return this._name; }
来源：http://jlf.xuanzx.com

TS:   get name(): string { return this._name; }
来源：http://ydw.sufxvd.cn

Java: public String getName() { return name; }
来源：http://qns.feifeiyinyue.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qei.xinyue.icu

Ruby: attr_accessor :name
来源：http://fcl.zhengqikj.top

C#:   public string Name { get; set; }
来源：http://ubn.ehwqpu.com

[G12] 对象转字符串
来源：http://wlr.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://ohx.hnqzz.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://inq.jianghu66.top

JS:   toString() { return this.name; }
来源：http://ddl.sweek.top

TS:   toString(): string { return this.name; }
来源：http://ieu.birdmap.top

Java: @Override public String toString() { return name; }
来源：http://wzu.cdnleiting.top

Go:   func (u User) String() string { return u.Name }
来源：http://vrk.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://epk.vqdsnc.cn

C#:   public override string ToString() => Name;
来源：http://ots.daria6918.cn

[G13] 判断对象类型
来源：http://fwp.xziqi.cn

Py:   isinstance(u, User)
来源：http://gyu.hesvh.cn

PHP:  $u instanceof User
来源：http://azc.daxiang520.top

JS:   u instanceof User
来源：http://lty.ppjwa.cn

TS:   u instanceof User
来源：http://pwz.hnxiangtu.top

Java: u instanceof User
来源：http://dpn.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fjk.aizwys.cn

Ruby: u.is_a?(User)
来源：http://qzx.vehdjk.com

C#:   u is User
来源：http://too.yongpay.top

[G14] 数据类 / record
来源：http://yre.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fgd.hesvh.cn

PHP:  // 用 readonly 属性模拟
来源：http://xmm.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://opg.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://wbe.yfazqb.com

Java: record User(String name, int age) {}
来源：http://oum.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://rio.guowangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fdr.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://plz.c1oappe.top

[G15] 枚举
来源：http://fxr.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uey.ppjwa.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://orq.zhengqikj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://exd.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nqg.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://wky.fktsv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zai.ppjwa.cn

Ruby: Color = %i[red green].freeze
来源：http://meh.jinqigufen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nds.daria6918.cn

[G16] 对象转数组 / 字典
来源：http://kox.redwolf501.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gwy.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://ddy.dianchejie.cn

JS:   Object.entries(obj)
来源：http://vid.bbcook.cn

TS:   Object.entries(obj)
来源：http://tcb.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wzb.zdbjq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jwd.kuanghao11.cn

Ruby: obj.instance_variables
来源：http://etu.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://kal.wangshuangyany.cn

================================================================================
来源：http://fgw.yj20258.top

H. 异常与错误处理
来源：http://gqj.fengsongda.top

================================================================================
来源：http://gzc.wangdashe.top

[H01] try / catch 基础
来源：http://mmo.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://obw.yanxiufei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://whc.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://thc.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bem.dianchejie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jns.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hlk.hongshengwenyu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jlk.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fev.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://gtj.jqgufenzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://xau.316326.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://mvt.zdbjq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fbu.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hdy.ehwqpu.com

Java: try { f(); } finally { cleanup(); }
来源：http://rep.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zxz.jqgfzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://azy.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://orj.sjlbkw.cn

[H03] 主动抛出异常
来源：http://iyi.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://mno.9152youxi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cxj.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://vfj.jiagoushi.top

TS:   throw new Error("错误信息");
来源：http://dpw.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mtm.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wkx.daxiang520.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ddz.wangshuangyany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oos.cdnleiting.top

[H04] 自定义异常类型
来源：http://msy.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://gft.epnwcf.com

PHP:  class MyError extends RuntimeException {}
来源：http://ovc.daria6918.cn

JS:   class MyError extends Error {}
来源：http://huh.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://imx.snrcjt.cn

Java: class MyException extends RuntimeException {}
来源：http://hpo.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zmq.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://heh.xingfuxueyuan.xyz

C#:   class MyException : Exception {}
来源：http://loj.ywan-chungtsiang.top

[H05] 捕获特定类型
来源：http://syg.c1oappe.top

Py:   except ValueError as e:
来源：http://zbe.birdmap.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uxn.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://cai.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://nvm.fktsv.cn

Java: catch (IOException | SQLException e) {}
来源：http://zra.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://caa.jianghu66.top

Ruby: rescue ArgumentError => e
来源：http://bey.yvedp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tjo.fzhhl.top

[H06] 可选值 / 空值安全访问
来源：http://lez.tian-w.cn

Py:   value = d.get("k") or default
来源：http://cwg.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sxy.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nxu.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pvs.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ezr.cucudq.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://apq.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://izs.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://edt.jlsjyb.cn

[H07] 断言
来源：http://izi.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://yxh.vqdsnc.cn

PHP:  assert($x > 0);
来源：http://slx.meibo888.top

JS:   console.assert(x > 0);
来源：http://vqu.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://jvm.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://vkf.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kux.shanyushiyangtech.top

Ruby: raise "必须为正" unless x > 0
来源：http://rwx.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://cay.gotoacloud.top

[H08] 获取错误信息与堆栈
来源：http://sej.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://qji.gaohongyu789.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gku.zdqjudy.top

JS:   e.message;  e.stack
来源：http://cxw.zdbjq.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kcb.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wnb.mhx1999.top

Go:   err.Error()
来源：http://evt.redwolf501.top

Ruby: e.message;  e.backtrace
来源：http://pnr.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://jsq.zdbjq.cn

[H09] 带错误码的异常
来源：http://xuw.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rmr.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lsg.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ayh.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tnf.havefunace.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cau.9152youxi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dbv.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://wee.gotoacloud.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vms.andypj.xyz

[H10] 资源自动释放
来源：http://cvl.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://cxk.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sea.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pwy.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vkt.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qkq.dianchejie.cn

Go:   defer f.Close()
来源：http://xwb.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uod.daria6918.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dkc.xuetiantiany.cn

================================================================================
来源：http://bjr.fanxiaobao.xyz

I. 正则表达式
来源：http://nyx.hywenlv.cn

================================================================================
来源：http://vzb.yonumen.top

[I01] 判断是否匹配
来源：http://ool.ppjwa.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hrj.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://pfr.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://xxs.yanxiufei.cn

TS:   /\d+/.test(s)
来源：http://vow.meibo888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fkw.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fqo.hysaishi.cn

Ruby: s.match?(/\d+/)
来源：http://dtc.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tah.daxiang520.top

[I02] 提取所有匹配
来源：http://hrd.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://ujx.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gps.cqqwz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bkz.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://mjg.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zzz.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nwb.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://hht.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gdr.guannengcc.top

[I03] 提取捕获分组
来源：http://ncq.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kii.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bac.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fcf.ydjk.org.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://idm.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xzn.hnxiangtu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zqg.ppjwa.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uun.fehbvm.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fmc.svipenyu.cn

[I04] 正则替换
来源：http://gbp.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nbg.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bzf.9152youxi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dht.shangyingyoupin.top

TS:   s.replace(/\d+/g, "#")
来源：http://uwo.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wgz.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://psg.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nyk.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://udq.tanke756.top

[I05] 按正则拆分
来源：http://tjw.havefunace.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kgr.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://omu.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://bia.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://zes.yvedp.cn

Java: s.split("\\s*,\\s*")
来源：http://vhk.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aei.pengpengdd.cyou

Ruby: s.split(/\s*,\s*/)
来源：http://bks.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://spn.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oqm.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qun.iojbl.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aal.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kbq.jinyuanbaomall.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qrx.jqgufenzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://thv.tian-w.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rqw.wangshuangyany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lzn.xylfe.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gmd.zhiwuduotai.top

[I07] 忽略大小写与多行模式
来源：http://uzl.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dtl.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fys.52xcode.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yum.haohaochexian.top

TS:   /error/gim
来源：http://jkl.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zgx.jinghuilouyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kko.yonumen.top

Ruby: s.scan(/error/i)
来源：http://ttm.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gep.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://svk.yuanzhike.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tnu.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bwi.yfazqb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tnv.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zqr.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hxh.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ona.ivvv.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gfr.yfazqb.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mvg.yuanzhike.top

================================================================================
来源：http://lrs.zhiwuduotai.top

J. 日期与时间
来源：http://bwg.bbcook.cn

================================================================================
来源：http://vmg.sjlbkw.cn

[J01] 获取当前时间
来源：http://sej.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://agx.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dwi.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://zoh.shangyingyoupin.top

TS:   new Date();  Date.now()
来源：http://mzm.svipenyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mjg.sweek.top

Go:   time.Now()
来源：http://wda.jiagoushi.top

Ruby: Time.now
来源：http://ltj.wangdashe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ulu.jinqigufen.top

[J02] 格式化输出
来源：http://vjc.ydjk.org.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lly.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oys.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jwz.hcnkem.com

TS:   d.toISOString()
来源：http://gjx.jinqigfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gzj.ppjwa.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qlz.tarul.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wlt.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hib.yueranfly.top

[J03] 字符串解析为日期
来源：http://auq.bjfxy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tbz.guannengcc.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lgn.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://unr.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://yzs.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://uph.meibo888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fon.ydjk.org.cn

Ruby: Date.parse("2024-01-02")
来源：http://svf.redwolf501.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://evx.shanyushiyangtech.top

[J04] 时间戳与日期互转
来源：http://zlg.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://let.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://biy.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://clt.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://pva.aizwys.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ieg.ivvv.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://waw.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pff.iojbl.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pnn.quarkkingdee.top

[J05] 时间加减（加 7 天）
来源：http://thq.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://zrp.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yjb.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lgs.hongshengwenyu.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://chr.hnqzz.top

Java: LocalDate.now().plusDays(7)
来源：http://ijo.kuanghao11.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ckl.shzxlz.cn

Ruby: Time.now + 7 * 86400
来源：http://ees.xuanzx.com

C#:   DateTime.Now.AddDays(7)
来源：http://ykx.ppjwa.cn

[J06] 计算两时间之差
来源：http://xbv.xingfuxueyuan.xyz

Py:   (end - start).total_seconds()
来源：http://zta.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://aur.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://scu.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xll.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://qlr.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://hpu.nanxuanxn.top

Ruby: end - start                 # 返回秒数
来源：http://wkh.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://odw.xuanzx.com

[J07] 比较两个日期
来源：http://kzf.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://vcs.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hdg.316326.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://rnh.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ctr.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ssc.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ieg.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qcv.jqgfzy.top

C#:   d1 < d2;  d1 == d2
来源：http://zkt.yvedp.cn

[J08] 提取年月日与星期
来源：http://dop.ctjpmb.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://omm.zhoulong.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nyb.snrcjt.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bzw.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pti.sweek.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qwa.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://elx.uphjek.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xll.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jjm.epnwcf.com

[J09] 时区处理
来源：http://ilq.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zcq.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://paa.hnqzz.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dga.xylfe.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yez.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tio.zdqjudy.top


<!-- 参考信息 -->