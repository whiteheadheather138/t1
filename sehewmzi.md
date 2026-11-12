代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mny.nanxinkj.top

[Q75] 日期格式化
来源：http://vuk.ppjwa.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://njs.gzhubu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wdn.nanxuanxn.top

[Q76] 按天统计
来源：http://cjf.xinyue.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://get.c1oappe.top

[Q77] 时间加减
来源：http://sxm.xuetiantiany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vae.wangshuangyany.cn

[Q78] 当前时间
来源：http://ebo.hnqzz.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ddp.yuxming.cn

[Q79] 字符串拼接
来源：http://frk.fzhhl.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uzu.yuxming.cn

[Q80] 字符串截取
来源：http://wry.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://shz.hnxiangtu.top

[Q81] 字符串替换
来源：http://mtp.yj20258.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://spu.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://mat.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jtg.pycfn.com

[Q83] 大小写转换
来源：http://wjp.pengpengdd.cyou

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oey.yj20258888.top

[Q84] 去除首尾空格
来源：http://nax.jlsjyb.cn

SELECT TRIM(name) FROM users;
来源：http://tqk.snrcjt.cn

[Q85] 数值取整
来源：http://xqt.mhx1999.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nbe.yj202588.top

[Q86] 读取 JSON 字段
来源：http://qlp.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kas.iojbl.cn

[Q87] JSON 字段做条件
来源：http://zcn.zhiwuduotai.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ynu.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://eaa.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://meq.ydjk.org.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xwe.shanyushiyangtech.top

[Q89] 判断表是否存在
来源：http://hbp.andypj.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://frc.zhengqikj.top

[Q90] 生成序号列
来源：http://lew.feifeiyinyue.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aae.hysaishi.cn

================================================================================
来源：http://pmw.xinyue.icu

R. Bash 专题
来源：http://bfa.dianchejie.cn

================================================================================
来源：http://mmi.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://act.fzhhl.top

#!/usr/bin/env bash
来源：http://wwh.c1oappe.top

set -euo pipefail
来源：http://mpb.xinyue.icu

[R02] 变量赋值与使用
来源：http://bzk.gogol.net.cn

name="Tom"; echo "$name"
来源：http://eft.shangyingyoupin.top

[R03] 只读变量
来源：http://axj.jianghu66.top

readonly PI=3.14
来源：http://fqz.redwolf501.top

[R04] 位置参数
来源：http://eou.jinyuanbaomall.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bdd.hesvh.cn

[R05] 参数默认值
来源：http://yar.jianghu66.top

name="${1:-default}"
来源：http://pbx.c1oappe.top

[R06] 判断命令是否存在
来源：http://oym.wangshuangyany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bcl.jinqigfzy.top

[R07] if 判断文件
来源：http://pjk.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://car.zhiwuduotai.top

[R08] 数值比较
来源：http://fyz.shangyingyoupin.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nvz.gaohongyu789.top

[R09] 字符串比较
来源：http://eqd.c1oappe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qdc.zycfv.cn

[R10] 正则匹配
来源：http://ilb.hesvh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pyz.hysaishi.cn

[R11] case 多分支
来源：http://qrd.shangyingyoupin.top

case "$1" in
来源：http://kco.vqdsnc.cn

start) echo "启动" ;;
来源：http://cbi.zycfv.cn

stop)  echo "停止" ;;
来源：http://mfa.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://dbp.52xcode.cn

esac
来源：http://rxn.zhengqikj.top

[R12] for 遍历文件
来源：http://atc.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://zxp.chenzaomai.com

[R13] for 计数循环
来源：http://gwo.zhijiandao.cn

for i in {1..10}; do echo "$i"; done
来源：http://soi.yj202588.top

[R14] C 风格 for
来源：http://yap.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ftx.daxiang520.top

[R15] while 逐行读文件
来源：http://lws.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bpv.tianlin.xyz

[R16] until 等待条件
来源：http://ola.shanyushiyangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oqh.wangdashe.top

[R17] 数组定义与取值
来源：http://kme.wangdashe.top

arr=(a b c); echo "${arr[0]}"
来源：http://cmj.9152youxi.cn

[R18] 遍历数组
来源：http://yer.ybcxt.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gfe.yueranfly.top

[R19] 数组长度
来源：http://lai.bbcook.cn

echo "${#arr[@]}"
来源：http://wpa.yangfankeji.com

[R20] 关联数组（字典）
来源：http://jlc.hysaishi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rdw.xinyue.icu

[R21] 字符串长度
来源：http://iac.gzhubu.top

echo "${#s}"
来源：http://ubb.sweek.top

[R22] 截取子串
来源：http://mmo.cqqwz.cn

echo "${s:0:5}"
来源：http://apx.zhixingplan.top

[R23] 字符串替换
来源：http://bdy.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xuj.shanyushiyangkeji.top

[R24] 大小写转换
来源：http://klx.0kj1m.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lmt.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://kfi.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uee.yongpay.top

[R26] 命令替换
来源：http://kon.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://qyc.hywenlv.cn

[R27] 算术展开
来源：http://mjd.aizwys.cn

echo $((1 + 2 * 3))
来源：http://wpy.haohaochexian.top

[R28] 浮点运算
来源：http://inu.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://fqw.9152youxi.cn

[R29] 定义函数
来源：http://ezi.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cxj.yongpay.top

[R30] 函数返回状态码
来源：http://whq.xuanzx.com

f() { return 0; }; f || echo "失败了"
来源：http://xlx.zdqjudy.top

[R31] 局部变量
来源：http://kvt.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://kvl.sxryk.cn

[R32] 参数个数校验
来源：http://ije.xinyue.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rgl.bbcook.cn

[R33] 捕获错误并提示行号
来源：http://wvv.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qau.hongshengwenyu.top

[R34] 退出时清理
来源：http://pez.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uop.cashguo.top

[R35] 后台执行并等待
来源：http://pma.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ear.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://brl.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dfr.cheryme.top

[R37] 把输出赋给变量
来源：http://syi.svipenyu.cn

files=$(ls -1)
来源：http://clv.yueranfly.top

[R38] 管道串联
来源：http://egk.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://yfg.zhaomingkeji.xyz

[R39] 重定向标准输出与错误
来源：http://toh.zycfv.cn

cmd > out.log 2>&1
来源：http://hne.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://tjo.zhoulong.xyz

echo "log" >> out.log
来源：http://itq.316326.xyz

[R41] 丢弃输出
来源：http://acn.guannengcc.top

cmd >/dev/null 2>&1
来源：http://nsx.snrcjt.cn

[R42] 输入重定向
来源：http://dik.yvedp.cn

wc -l < a.txt
来源：http://xlf.zhixingplan.top

[R43] 按名字查找文件
来源：http://vku.c1oappe.top

find . -name "*.log" -type f
来源：http://hqq.nanxinkj.top

[R44] 按修改时间查找
来源：http://rbh.daxiang520.top

find . -mtime -7 -type f
来源：http://huj.hnxiangtu.top

[R45] 批量删除
来源：http://lqk.ydjk.org.cn

find . -name "*.tmp" -delete
来源：http://evq.jqgufenzy.top

[R46] 递归替换文件内容
来源：http://wwi.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hza.feifeiyinyue.top

[R47] sed 单行替换
来源：http://iuh.pengpengdd.cyou

sed -i 's/foo/bar/g' a.txt
来源：http://sjw.epnwcf.com

[R48] awk 取指定列
来源：http://vll.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://hnt.gotoacloud.top

[R49] awk 带条件
来源：http://ytg.smart0.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ktr.hesvh.cn

[R50] awk 求和
来源：http://lce.yonumen.top

awk '{s += $2} END {print s}' a.txt
来源：http://ufu.nanxuanxn.top

[R51] 排序去重取前几
来源：http://agx.jlsjyb.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://byk.zhongyouzk.top

[R52] 统计行数
来源：http://wkk.chenjidiqi.icu

wc -l a.txt
来源：http://omm.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://jjd.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xxo.52xcode.cn

[R54] 比较两个文件
来源：http://ynk.ydjk.org.cn

diff a.txt b.txt
来源：http://jjs.yj202588.top

[R55] 压缩与解压
来源：http://fkh.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gxb.yj202588.top

[R56] 远程拷贝
来源：http://kyq.shanyushiyangtech.top

scp file user@host:/path/
来源：http://lfh.hcnkem.com

[R57] 远程执行命令
来源：http://ooi.yongpay.top

ssh user@host 'uptime'
来源：http://rxs.xingfuxueyuan.xyz

[R58] 下载文件
来源：http://yeh.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://whb.sxryk.cn

[R59] 发 POST JSON
来源：http://cvm.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mhm.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://fek.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://col.vqdsnc.cn

[R61] 磁盘占用
来源：http://txm.chenjidiqi.icu

df -h;  du -sh *
来源：http://zqx.chenlongwang.top

[R62] 找最占空间的文件
来源：http://bcg.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://gpz.feifeiyinyue.top

[R63] 内存与进程
来源：http://mmg.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://vox.chenjidiqi.icu

[R64] 结束进程
来源：http://aov.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://diu.epnwcf.com

[R65] 查看端口占用
来源：http://owu.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ylw.kuanghao11.cn

[R66] 定时任务
来源：http://hta.mhx1999.top

crontab -e;  crontab -l
来源：http://ank.zdqjudy.top

[R67] 生成随机十六进制串
来源：http://xos.cdnleiting.top

openssl rand -hex 16
来源：http://gdw.zhaomingkeji.xyz

[R68] 计算文件校验值
来源：http://xaj.yj202588.top

sha256sum a.txt;  md5sum a.txt
来源：http://qmh.yanxiufei.cn

[R69] 生成随机密码
来源：http://bgy.ydjk.org.cn

head -c 16 /dev/urandom | base64
来源：http://ufz.zhengqikj.top

[R70] 时间戳与互转
来源：http://qbj.fengsongda.top

date +%s;  date -d @1700000000
来源：http://znu.yongpay.top

[R71] 日期格式化
来源：http://zsp.yfazqb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://bgx.xingfuxueyuan.xyz

[R72] 等待端口就绪
来源：http://cha.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hfx.hysaishi.cn

[R73] 分割大日志
来源：http://aqk.pycfn.com

split -l 1000 big.log part_
来源：http://pxr.vehdjk.com

[R74] 批量重命名
来源：http://msi.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vix.uphjek.com

[R75] 导出环境变量
来源：http://dye.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://iuw.xinyue.icu

[R76] 使用临时文件
来源：http://ycm.hnqzz.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pce.gzhubu.top

[R77] 读取用户输入
来源：http://jzu.redwolf501.top

read -rp "请输入: " ans
来源：http://mmg.xziqi.cn

[R78] 交互式菜单
来源：http://hgy.aibaodan.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nnf.dashuyun.cn

[R79] 解析命令行选项
来源：http://kon.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fhd.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://qtg.ywan-chungtsiang.top

time ./run.sh
来源：http://yku.hongshengwenyu.top

================================================================================
来源：http://aqd.zdbjq.cn

S. C / C++ 专题
来源：http://umw.yj20258888.top

================================================================================
来源：http://rpk.zhixingplan.top

[S01] C：Hello World
来源：http://jph.yongpay.top

#include <stdio.h>
来源：http://kpw.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rsf.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://dkj.ydzc1.top

int a = 10; printf("%d\n", a);
来源：http://oth.gotoacloud.top

[S03] C：读入整数
来源：http://orc.c1oappe.top

int x; scanf("%d", &x);
来源：http://sgu.gaohongyu789.top

[S04] C：字符串复制
来源：http://ltl.jqgfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://zfv.yuxming.cn

[S05] C：字符串长度
来源：http://jzb.zdqjudy.top

strlen(s)
来源：http://vor.yuxming.cn

[S06] C：字符串比较
来源：http://jzc.svipenyu.cn

strcmp(a, b) == 0
来源：http://isi.zhixingplan.top

[S07] C：数组遍历求和
来源：http://qtn.zhaomingkeji.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://irp.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://bfy.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dzm.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://lxl.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://apw.jianghu66.top

[S10] C：指针与解引用
来源：http://egi.pycfn.com

int *p = &a;  *p = 5;
来源：http://qjx.jinqigufen.top

[S11] C：逐行读文件
来源：http://cjm.fengsongda.top

FILE *f = fopen("a.txt", "r");
来源：http://cew.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jwt.ywan-chungtsiang.top

fclose(f);
来源：http://xuq.dashuyun.cn

[S12] C：写文件
来源：http://occ.shanyushiyangtech.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hch.cqqwz.cn

[S13] C：宏定义
来源：http://aog.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wcu.ehwqpu.com

[S14] C：枚举
来源：http://yuc.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://vck.yuxming.cn

[S15] C：类型转换
来源：http://nqd.xuetiantiany.cn

(double) a / b
来源：http://udp.yvedp.cn

[S16] C：位操作置位
来源：http://iwa.nwbrower.top

x |= (1 << 3);
来源：http://fgr.svipenyu.cn

[S17] C：安全拼接字符串
来源：http://wqm.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qol.sysykeji.top

[S18] C：命令行参数
来源：http://itw.havefunace.top

int main(int argc, char **argv)
来源：http://klx.fktsv.cn

[S19] C：快速排序
来源：http://uww.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://mhs.jlsjyb.cn

[S20] C：二分查找
来源：http://ppl.hnqzz.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nui.shangyingyoupin.top

[S21] C：字符类别判断
来源：http://hhj.svipenyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qmr.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://xwj.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://qke.sxryk.cn

[S23] C：随机数
来源：http://ytj.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://kiv.ctjpmb.com

[S24] C：获取本地时间
来源：http://nap.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kcm.yuanzhike.top

[S25] C：内存拷贝
来源：http://zst.cucudq.cn

memcpy(dst, src, n);
来源：http://zad.shuidangran.top

[S26] C：内存清零
来源：http://pmx.cdnleiting.top

memset(a, 0, sizeof a);
来源：http://wcr.zhoulong.xyz

[S27] C：定义常量
来源：http://pfu.cucudq.cn

const double PI = 3.14159;
来源：http://qav.quarkkingdee.top

[S28] C：静态变量
来源：http://old.chenjidiqi.icu

static int counter = 0;
来源：http://ida.zhijiandao.cn

[S29] C：变参函数
来源：http://zya.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uuq.quarkkingdee.top

[S30] C：头文件保护
来源：http://uib.ehwqpu.com

#ifndef X_H
来源：http://ljq.ehwqpu.com

#define X_H
来源：http://nfu.birdmap.top

#endif
来源：http://tci.daxiang520.top

[S31] C++：Hello World
来源：http://lhm.zhengqikj.top

#include <iostream>
来源：http://dnn.tian-w.cn

int main() { std::cout << "Hello\n"; }
来源：http://jhd.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://rbn.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://agl.svipenyu.cn

[S33] C++：vector 增删
来源：http://tew.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://roa.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://qbv.52xcode.cn

for (auto &x : v) { std::cout << x; }
来源：http://qfo.hammf.cn

[S35] C++：map
来源：http://ftb.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ekh.gaohongyu789.top

[S36] C++：unordered_map
来源：http://mql.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://otl.jqgufenzy.top

[S37] C++：set
来源：http://szs.ybcxt.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nop.yonumen.top

[S38] C++：排序
来源：http://kbu.gogol.net.cn

std::sort(v.begin(), v.end());
来源：http://xmk.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://gtq.jqgfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ckb.gotoacloud.top

[S40] C++：查找元素
来源：http://aam.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ftf.wangdashe.top

[S41] C++：类与构造函数
来源：http://fnv.hnqzz.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kqk.tianlin.xyz

[S42] C++：继承与虚函数
来源：http://ilf.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://vkk.ctjpmb.com

[S43] C++：智能指针
来源：http://mrn.fanxiaobao.xyz

auto p = std::make_unique<int>(5);
来源：http://lwf.hnqzz.top

[S44] C++：引用传参
来源：http://zhc.jiagoushi.top

void inc(int &x) { ++x; }
来源：http://bbu.ydjk.org.cn


<!-- 参考信息 -->