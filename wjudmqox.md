代发 wailian999

SHOW INDEX FROM users;
来源：http://nkf.c1oappe.top

[Q73] 查看表状态
来源：http://vzu.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gse.iojbl.cn

[Q74] 强制使用索引
来源：http://mnr.xylfe.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ses.tanke756.top

[Q75] 日期格式化
来源：http://rti.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kja.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yvx.hammf.cn

[Q76] 按天统计
来源：http://xbo.yangfankeji.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://era.yuanzhike.top

[Q77] 时间加减
来源：http://qfo.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ikz.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://wql.fehbvm.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dcf.shanyushiyangtech.top

[Q79] 字符串拼接
来源：http://yfy.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vst.xingfuxueyuan.xyz

[Q80] 字符串截取
来源：http://pvk.xziqi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tnd.sjlbkw.cn

[Q81] 字符串替换
来源：http://ugd.ywan-chungtsiang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lgd.aibaodan.cn

[Q82] 字符长度与字节长度
来源：http://mlh.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://avb.tanke756.top

[Q83] 大小写转换
来源：http://jdk.iojbl.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cxo.wangdashe.top

[Q84] 去除首尾空格
来源：http://ysk.sweek.top

SELECT TRIM(name) FROM users;
来源：http://iuj.zhixingplan.top

[Q85] 数值取整
来源：http://use.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wxx.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://edt.hnqzz.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jtw.cashguo.top

[Q87] JSON 字段做条件
来源：http://ryp.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yrj.kuanghao11.cn

[Q88] 行转列（条件聚合）
来源：http://tuv.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vkd.9152youxi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oek.snrcjt.cn

[Q89] 判断表是否存在
来源：http://hyk.mhx1999.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ooe.gotoacloud.top

[Q90] 生成序号列
来源：http://rzg.guowangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://phk.redwolf501.top

================================================================================
来源：http://pxh.ydzc1.top

R. Bash 专题
来源：http://kru.yanxiufei.cn

================================================================================
来源：http://nzr.shzxlz.cn

[R01] shebang 与严格模式
来源：http://ytk.hysaishi.cn

#!/usr/bin/env bash
来源：http://jvb.sysykeji.top

set -euo pipefail
来源：http://nye.guowangkeji.top

[R02] 变量赋值与使用
来源：http://ipz.tanke756.top

name="Tom"; echo "$name"
来源：http://kfl.zhoulong.xyz

[R03] 只读变量
来源：http://fya.mhx1999.top

readonly PI=3.14
来源：http://lmk.aibaodan.cn

[R04] 位置参数
来源：http://suo.jinyuanbaomall.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eqw.zhaomingkeji.xyz

[R05] 参数默认值
来源：http://gru.birdmap.top

name="${1:-default}"
来源：http://vpi.zhixingplan.top

[R06] 判断命令是否存在
来源：http://lua.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aqa.wangshuangyany.cn

[R07] if 判断文件
来源：http://opi.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gxa.gogol.net.cn

[R08] 数值比较
来源：http://lhk.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://vhp.sufxvd.cn

[R09] 字符串比较
来源：http://xcq.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zsg.hammf.cn

[R10] 正则匹配
来源：http://bso.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wmg.tarul.cn

[R11] case 多分支
来源：http://ndh.tarul.cn

case "$1" in
来源：http://xop.52xcode.cn

start) echo "启动" ;;
来源：http://tnq.yj20258888.top

stop)  echo "停止" ;;
来源：http://thz.haohaochexian.top

*)     echo "未知命令" ;;
来源：http://bji.jinghuilouyu.cn

esac
来源：http://qha.chenlongwang.top

[R12] for 遍历文件
来源：http://sas.cucudq.cn

for f in *.txt; do echo "$f"; done
来源：http://fbr.bjfxy.top

[R13] for 计数循环
来源：http://vwh.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://xtm.hesvh.cn

[R14] C 风格 for
来源：http://ztn.zhoulong.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mis.shuidangran.top

[R15] while 逐行读文件
来源：http://kew.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://glo.hesvh.cn

[R16] until 等待条件
来源：http://uuo.yj202588.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ocs.hongshengwenyu.top

[R17] 数组定义与取值
来源：http://vdr.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gof.hywenlv.cn

[R18] 遍历数组
来源：http://hsg.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iri.jinghuilouyu.cn

[R19] 数组长度
来源：http://gvb.xuetiantiany.cn

echo "${#arr[@]}"
来源：http://udc.andypj.xyz

[R20] 关联数组（字典）
来源：http://xgi.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ycs.chenlongwang.top

[R21] 字符串长度
来源：http://fxb.sufxvd.cn

echo "${#s}"
来源：http://drs.gzhubu.top

[R22] 截取子串
来源：http://kqx.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://eti.shangyingyoupin.top

[R23] 字符串替换
来源：http://szq.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dar.wangshuangyany.cn

[R24] 大小写转换
来源：http://nkw.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://cek.sxryk.cn

[R25] 去后缀 / 去前缀
来源：http://opt.uphjek.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://zzy.zdbjq.cn

[R26] 命令替换
来源：http://lik.bjfxy.top

now=$(date +%F); echo "$now"
来源：http://jsy.havefunace.top

[R27] 算术展开
来源：http://nmp.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://qwy.chenlongwang.top

[R28] 浮点运算
来源：http://fno.ywan-chungtsiang.top

echo "scale=2; 10/3" | bc
来源：http://ahq.tarul.cn

[R29] 定义函数
来源：http://ylr.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hmr.hfpthk.cn

[R30] 函数返回状态码
来源：http://pjc.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://bgu.yfazqb.com

[R31] 局部变量
来源：http://dpb.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://boi.0kj1m.cn

[R32] 参数个数校验
来源：http://fim.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ubt.smart0.xyz

[R33] 捕获错误并提示行号
来源：http://mmq.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uij.vqdsnc.cn

[R34] 退出时清理
来源：http://rgi.nwbrower.top

trap 'rm -f "$tmp"' EXIT
来源：http://ogk.vehdjk.com

[R35] 后台执行并等待
来源：http://xwz.cucudq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fvb.ydzc1.top

[R36] 并发执行多个任务
来源：http://arz.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vhq.guannengcc.top

[R37] 把输出赋给变量
来源：http://mhu.fengsongda.top

files=$(ls -1)
来源：http://zdq.guannengcc.top

[R38] 管道串联
来源：http://ddf.sxryk.cn

cat a.txt | grep -i error | wc -l
来源：http://jku.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://wha.jqgufenzy.top

cmd > out.log 2>&1
来源：http://hjv.zdqjudy.top

[R40] 追加写日志
来源：http://zgt.gaohongyu789.top

echo "log" >> out.log
来源：http://hex.guannengcc.top

[R41] 丢弃输出
来源：http://dld.bbcook.cn

cmd >/dev/null 2>&1
来源：http://rui.zycfv.cn

[R42] 输入重定向
来源：http://quo.ybcxt.top

wc -l < a.txt
来源：http://tfk.hammf.cn

[R43] 按名字查找文件
来源：http://mhi.sxryk.cn

find . -name "*.log" -type f
来源：http://evz.hongshengwenyu.top

[R44] 按修改时间查找
来源：http://gxl.zdqjudy.top

find . -mtime -7 -type f
来源：http://gci.yj20258888.top

[R45] 批量删除
来源：http://ojc.sufxvd.cn

find . -name "*.tmp" -delete
来源：http://yqk.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://vjc.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fpc.zdbjq.cn

[R47] sed 单行替换
来源：http://wbu.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://mkz.hysaishi.cn

[R48] awk 取指定列
来源：http://jul.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://bzl.fanxiaobao.xyz

[R49] awk 带条件
来源：http://jzx.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dij.xuanzx.com

[R50] awk 求和
来源：http://pkb.chenlongwang.top

awk '{s += $2} END {print s}' a.txt
来源：http://exm.zhengqikj.top

[R51] 排序去重取前几
来源：http://etx.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://svl.pengpengdd.cyou

[R52] 统计行数
来源：http://sfo.jinyuanbaomall.cn

wc -l a.txt
来源：http://lkl.yonumen.top

[R53] 查看文件头与实时尾
来源：http://zct.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ici.shzxlz.cn

[R54] 比较两个文件
来源：http://drt.cucudq.cn

diff a.txt b.txt
来源：http://nly.jqgfzy.top

[R55] 压缩与解压
来源：http://owu.yuanzhike.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://skp.zhengqikj.top

[R56] 远程拷贝
来源：http://pld.guowangkeji.top

scp file user@host:/path/
来源：http://ebe.meibo888.top

[R57] 远程执行命令
来源：http://ovv.sweek.top

ssh user@host 'uptime'
来源：http://wre.dianchejie.cn

[R58] 下载文件
来源：http://wul.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://swg.guannengcc.top

[R59] 发 POST JSON
来源：http://tlq.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kxi.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://fiv.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hzu.zhoulong.xyz

[R61] 磁盘占用
来源：http://iea.cucudq.cn

df -h;  du -sh *
来源：http://wez.zhengqikj.top

[R62] 找最占空间的文件
来源：http://rxa.hnxiangtu.top

du -ah . | sort -rh | head -10
来源：http://nya.nanxinkj.top

[R63] 内存与进程
来源：http://zsz.jiagoushi.top

free -h;  ps aux | grep nginx
来源：http://biy.yongpay.top

[R64] 结束进程
来源：http://fzt.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://azj.bjfxy.top

[R65] 查看端口占用
来源：http://yvy.zdqjudy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iqk.hnxiangtu.top

[R66] 定时任务
来源：http://rgj.hnxiangtu.top

crontab -e;  crontab -l
来源：http://jlc.fzhhl.top

[R67] 生成随机十六进制串
来源：http://qit.zhijiandao.cn

openssl rand -hex 16
来源：http://dvc.hywenlv.cn

[R68] 计算文件校验值
来源：http://uln.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://zac.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://faq.iojbl.cn

head -c 16 /dev/urandom | base64
来源：http://bez.xinyue.icu

[R70] 时间戳与互转
来源：http://pxb.fzhhl.top

date +%s;  date -d @1700000000
来源：http://evf.ywan-chungtsiang.top

[R71] 日期格式化
来源：http://kjd.nanxuanxn.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zdc.yueranfly.top

[R72] 等待端口就绪
来源：http://zro.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fps.gotoacloud.top

[R73] 分割大日志
来源：http://jfz.zycfv.cn

split -l 1000 big.log part_
来源：http://jyv.guowangkeji.top

[R74] 批量重命名
来源：http://yfl.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ync.hcnkem.com

[R75] 导出环境变量
来源：http://dyd.bjfxy.top

export PATH="$HOME/bin:$PATH"
来源：http://kmt.fehbvm.com

[R76] 使用临时文件
来源：http://xui.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pft.gzhubu.top

[R77] 读取用户输入
来源：http://rkt.zhixingplan.top

read -rp "请输入: " ans
来源：http://xlv.iojbl.cn

[R78] 交互式菜单
来源：http://glu.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zoc.hesvh.cn

[R79] 解析命令行选项
来源：http://eja.zhengqikj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uez.yonumen.top

[R80] 查看脚本执行耗时
来源：http://cxf.52xcode.cn

time ./run.sh
来源：http://pgc.jinqigfzy.top

================================================================================
来源：http://yoz.ydzc1.top

S. C / C++ 专题
来源：http://pzf.gogol.net.cn

================================================================================
来源：http://sfj.yuxming.cn

[S01] C：Hello World
来源：http://oll.yj20258.top

#include <stdio.h>
来源：http://wks.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wsm.pycfn.com

[S02] C：变量与格式化输出
来源：http://lwa.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://dnk.jinqigfzy.top

[S03] C：读入整数
来源：http://wwl.ppjwa.cn

int x; scanf("%d", &x);
来源：http://eip.sysykeji.top

[S04] C：字符串复制
来源：http://lfa.yj20258888.top

char dst[32]; strcpy(dst, "hi");
来源：http://vqd.sysykeji.top

[S05] C：字符串长度
来源：http://rzt.zdbjq.cn

strlen(s)
来源：http://wje.zhoulong.xyz

[S06] C：字符串比较
来源：http://zom.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://mwm.cdnleiting.top

[S07] C：数组遍历求和
来源：http://ysi.c1oappe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nso.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://tjm.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kaa.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://xpc.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xju.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://ckk.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://jem.xuanzx.com

[S11] C：逐行读文件
来源：http://mgo.vehdjk.com

FILE *f = fopen("a.txt", "r");
来源：http://kii.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vcu.sufxvd.cn

fclose(f);
来源：http://ubb.jyoumei.cn

[S12] C：写文件
来源：http://obb.redwolf501.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lte.quarkkingdee.top

[S13] C：宏定义
来源：http://vqg.chenlongwang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vzw.jinyuanbaomall.cn

[S14] C：枚举
来源：http://kcp.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://fti.hongshengwenyu.top

[S15] C：类型转换
来源：http://jtg.shzxlz.cn

(double) a / b
来源：http://lbf.wangdashe.top

[S16] C：位操作置位
来源：http://gqb.wangshuangyany.cn

x |= (1 << 3);
来源：http://sye.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://irc.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ddl.haohaochexian.top

[S18] C：命令行参数
来源：http://kxa.yongpay.top

int main(int argc, char **argv)
来源：http://crj.yonumen.top

[S19] C：快速排序
来源：http://pem.yfazqb.com

qsort(a, n, sizeof(int), cmp);
来源：http://shx.jqgfzy.top

[S20] C：二分查找
来源：http://ckw.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ohu.gogol.net.cn

[S21] C：字符类别判断
来源：http://ccd.52xcode.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://csn.hnxiangtu.top

[S22] C：字符串转数字
来源：http://vim.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xgh.hnqzz.top

[S23] C：随机数
来源：http://wpc.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dzt.zhijiandao.cn

[S24] C：获取本地时间
来源：http://hij.c1oappe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mll.havefunace.top

[S25] C：内存拷贝
来源：http://hwe.haohaochexian.top

memcpy(dst, src, n);
来源：http://xmf.tianlin.xyz

[S26] C：内存清零
来源：http://vxi.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://vze.ehwqpu.com

[S27] C：定义常量
来源：http://xyz.yuxming.cn

const double PI = 3.14159;
来源：http://bcx.gotoacloud.top

[S28] C：静态变量
来源：http://coi.smart0.xyz

static int counter = 0;
来源：http://amm.zhoulong.xyz

[S29] C：变参函数
来源：http://gxm.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sss.daria6918.cn

[S30] C：头文件保护
来源：http://drp.gogol.net.cn

#ifndef X_H
来源：http://myz.zhongyouzk.top

#define X_H
来源：http://vap.fktsv.cn

#endif
来源：http://wbk.fktsv.cn

[S31] C++：Hello World
来源：http://bfb.hnqzz.top

#include <iostream>
来源：http://jjp.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://qmu.guowangkeji.top

[S32] C++：字符串
来源：http://yad.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://efw.chenjidiqi.icu

[S33] C++：vector 增删
来源：http://xwo.zhongyouzk.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jdb.yj20258.top

[S34] C++：遍历 vector
来源：http://ayo.meibo888.top

for (auto &x : v) { std::cout << x; }
来源：http://wsn.c1oappe.top

[S35] C++：map
来源：http://qbi.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://djc.ybcxt.top

[S36] C++：unordered_map
来源：http://far.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fgy.uphjek.com

[S37] C++：set
来源：http://ohh.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eia.bjfxy.top

[S38] C++：排序
来源：http://lni.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://cze.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://lme.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eyu.yangfankeji.com

[S40] C++：查找元素
来源：http://pqy.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eef.nanxinkj.top

[S41] C++：类与构造函数
来源：http://wrr.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vwv.zhixingplan.top

[S42] C++：继承与虚函数
来源：http://wfe.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://ury.zdqjudy.top


<!-- 参考信息 -->