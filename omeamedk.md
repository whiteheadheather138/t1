代发 wailian999

[Q63] 开启事务
来源：http://vak.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://iez.mhx1999.top

[Q64] 提交事务
来源：http://gxe.shanyushiyangtech.top

COMMIT;
来源：http://grw.xziqi.cn

[Q65] 回滚事务
来源：http://zxt.shangyingyoupin.top

ROLLBACK;
来源：http://bos.tian-w.cn

[Q66] 行锁查询
来源：http://qkh.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dlq.yuanzhike.top

[Q67] 设置隔离级别
来源：http://tpa.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kag.jinqigfzy.top

[Q68] 保存点
来源：http://kfv.gotoacloud.top

SAVEPOINT sp1;
来源：http://uzy.dashuyun.cn

ROLLBACK TO sp1;
来源：http://wem.bbcook.cn

[Q69] 查看执行计划
来源：http://qsq.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fth.cqqwz.cn

[Q70] 更新统计信息
来源：http://eer.xylfe.cn

ANALYZE TABLE users;
来源：http://nye.cdnleiting.top

[Q71] 查看建表语句
来源：http://zlo.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bsm.hfpthk.cn

[Q72] 查看索引
来源：http://qcf.316326.xyz

SHOW INDEX FROM users;
来源：http://jnb.sufxvd.cn

[Q73] 查看表状态
来源：http://yuu.havefunace.top

SHOW TABLE STATUS LIKE 'users';
来源：http://chm.uphjek.com

[Q74] 强制使用索引
来源：http://jmf.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fns.nanxinkj.top

[Q75] 日期格式化
来源：http://exr.yongpay.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uxc.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bcj.tanke756.top

[Q76] 按天统计
来源：http://fcw.daria6918.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tnu.svipenyu.cn

[Q77] 时间加减
来源：http://hug.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kyz.nwbrower.top

[Q78] 当前时间
来源：http://qhl.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://skg.jinqigufen.top

[Q79] 字符串拼接
来源：http://yus.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://etg.redwolf501.top

[Q80] 字符串截取
来源：http://uku.tanke756.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fkf.shangyingyoupin.top

[Q81] 字符串替换
来源：http://fap.gogol.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cpm.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://hqi.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pyv.smart0.xyz

[Q83] 大小写转换
来源：http://ghd.dianchejie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ufz.guowangkeji.top

[Q84] 去除首尾空格
来源：http://tnv.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://vrh.yongpay.top

[Q85] 数值取整
来源：http://lzq.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vgu.cheryme.top

[Q86] 读取 JSON 字段
来源：http://phr.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zkf.sysykeji.top

[Q87] JSON 字段做条件
来源：http://jfa.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hrp.hfpthk.cn

[Q88] 行转列（条件聚合）
来源：http://jdn.jlsjyb.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://alf.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mhw.meibo888.top

[Q89] 判断表是否存在
来源：http://ekx.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bqn.daxiang520.top

[Q90] 生成序号列
来源：http://piu.xingfuxueyuan.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uqx.shzxlz.cn

================================================================================
来源：http://zwu.fzhhl.top

R. Bash 专题
来源：http://fmv.zhijiandao.cn

================================================================================
来源：http://bck.mhx1999.top

[R01] shebang 与严格模式
来源：http://kcb.aibaodan.cn

#!/usr/bin/env bash
来源：http://gpt.quarkkingdee.top

set -euo pipefail
来源：http://abz.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://fit.9152youxi.cn

name="Tom"; echo "$name"
来源：http://ive.jiagoushi.top

[R03] 只读变量
来源：http://tvv.shanyushiyangkeji.top

readonly PI=3.14
来源：http://azc.yj20258888.top

[R04] 位置参数
来源：http://qzx.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bjp.cheryme.top

[R05] 参数默认值
来源：http://lyw.hnqzz.top

name="${1:-default}"
来源：http://zib.hammf.cn

[R06] 判断命令是否存在
来源：http://saj.ywan-chungtsiang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oag.jinyuanbaomall.cn

[R07] if 判断文件
来源：http://bpu.yuanzhike.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zig.iojbl.cn

[R08] 数值比较
来源：http://owz.hnxiangtu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cms.sysykeji.top

[R09] 字符串比较
来源：http://dfn.yueranfly.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://voe.hnxiangtu.top

[R10] 正则匹配
来源：http://mkq.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mrr.mhx1999.top

[R11] case 多分支
来源：http://abz.gogol.net.cn

case "$1" in
来源：http://flc.gotoacloud.top

start) echo "启动" ;;
来源：http://zqx.cqqwz.cn

stop)  echo "停止" ;;
来源：http://uti.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://oez.xinyue.icu

esac
来源：http://bks.tianlin.xyz

[R12] for 遍历文件
来源：http://mlp.yj20258888.top

for f in *.txt; do echo "$f"; done
来源：http://ikb.pycfn.com

[R13] for 计数循环
来源：http://mzs.tanke756.top

for i in {1..10}; do echo "$i"; done
来源：http://pdm.hywenlv.cn

[R14] C 风格 for
来源：http://mwf.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fho.hammf.cn

[R15] while 逐行读文件
来源：http://fiz.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vop.zdbjq.cn

[R16] until 等待条件
来源：http://iwy.shanyushiyangtech.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://abd.hfpthk.cn

[R17] 数组定义与取值
来源：http://suc.mhx1999.top

arr=(a b c); echo "${arr[0]}"
来源：http://qep.yanxiufei.cn

[R18] 遍历数组
来源：http://lab.gaohongyu789.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vwx.shanyushiyangtech.top

[R19] 数组长度
来源：http://xkx.tarul.cn

echo "${#arr[@]}"
来源：http://ovm.ehwqpu.com

[R20] 关联数组（字典）
来源：http://blo.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://knm.haohaochexian.top

[R21] 字符串长度
来源：http://set.ppjwa.cn

echo "${#s}"
来源：http://vau.cdnleiting.top

[R22] 截取子串
来源：http://zcd.fehbvm.com

echo "${s:0:5}"
来源：http://dtw.xinyue.icu

[R23] 字符串替换
来源：http://pxg.zhiwuduotai.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pmq.yongpay.top

[R24] 大小写转换
来源：http://sdg.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://zww.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://pvb.shangyingyoupin.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tsg.xuetiantiany.cn

[R26] 命令替换
来源：http://opc.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://gaw.316326.xyz

[R27] 算术展开
来源：http://sbg.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://psa.yvedp.cn

[R28] 浮点运算
来源：http://xht.shangyingyoupin.top

echo "scale=2; 10/3" | bc
来源：http://dpn.wangshuangyany.cn

[R29] 定义函数
来源：http://jjw.bjfxy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ssl.yj202588.top

[R30] 函数返回状态码
来源：http://qwj.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://bin.zhaomingkeji.xyz

[R31] 局部变量
来源：http://boq.yj20258.top

f() { local x=1; echo "$x"; }
来源：http://ajc.xuetiantiany.cn

[R32] 参数个数校验
来源：http://vni.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tbw.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://irr.chenzaomai.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nlz.9152youxi.cn

[R34] 退出时清理
来源：http://ypv.havefunace.top

trap 'rm -f "$tmp"' EXIT
来源：http://sqh.bjfxy.top

[R35] 后台执行并等待
来源：http://hrl.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xgd.bbcook.cn

[R36] 并发执行多个任务
来源：http://ezs.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dfx.jiagoushi.top

[R37] 把输出赋给变量
来源：http://ebl.yj202588.top

files=$(ls -1)
来源：http://mdl.zhoulong.xyz

[R38] 管道串联
来源：http://azs.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://wki.ivvv.top

[R39] 重定向标准输出与错误
来源：http://otg.ybcxt.top

cmd > out.log 2>&1
来源：http://vyv.kuanghao11.cn

[R40] 追加写日志
来源：http://jst.dianchejie.cn

echo "log" >> out.log
来源：http://ddy.zycfv.cn

[R41] 丢弃输出
来源：http://bcq.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://qev.zycfv.cn

[R42] 输入重定向
来源：http://trd.havefunace.top

wc -l < a.txt
来源：http://wyz.52xcode.cn

[R43] 按名字查找文件
来源：http://dfc.zhaomingkeji.xyz

find . -name "*.log" -type f
来源：http://zdr.hfpthk.cn

[R44] 按修改时间查找
来源：http://idn.zhengqikj.top

find . -mtime -7 -type f
来源：http://tga.ppjwa.cn

[R45] 批量删除
来源：http://qvx.0kj1m.cn

find . -name "*.tmp" -delete
来源：http://tld.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://qie.havefunace.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dcg.daxiang520.top

[R47] sed 单行替换
来源：http://hms.gotoacloud.top

sed -i 's/foo/bar/g' a.txt
来源：http://gei.sxryk.cn

[R48] awk 取指定列
来源：http://mzr.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://hff.hnxiangtu.top

[R49] awk 带条件
来源：http://vfi.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://slv.guowangkeji.top

[R50] awk 求和
来源：http://bxt.zhaomingkeji.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://wvp.bjfxy.top

[R51] 排序去重取前几
来源：http://uaf.zhijiandao.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mxb.guowangkeji.top

[R52] 统计行数
来源：http://ord.zhengqikj.top

wc -l a.txt
来源：http://tck.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://hep.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://akm.yj20258888.top

[R54] 比较两个文件
来源：http://urx.ydzc1.top

diff a.txt b.txt
来源：http://zid.yj20258888.top

[R55] 压缩与解压
来源：http://qtp.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hiz.fengsongda.top

[R56] 远程拷贝
来源：http://kci.tianlin.xyz

scp file user@host:/path/
来源：http://zma.bjfxy.top

[R57] 远程执行命令
来源：http://vol.zhijiandao.cn

ssh user@host 'uptime'
来源：http://vvn.ywan-chungtsiang.top

[R58] 下载文件
来源：http://jxy.daxiang520.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zek.snrcjt.cn

[R59] 发 POST JSON
来源：http://fhr.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://toe.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://wqy.dianchejie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zbe.gotoacloud.top

[R61] 磁盘占用
来源：http://oue.shzxlz.cn

df -h;  du -sh *
来源：http://rsr.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://ffu.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://lci.hfpthk.cn

[R63] 内存与进程
来源：http://vgl.zhaomingkeji.xyz

free -h;  ps aux | grep nginx
来源：http://uey.tarul.cn

[R64] 结束进程
来源：http://gvi.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://kbr.hywenlv.cn

[R65] 查看端口占用
来源：http://dzh.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tft.yangfankeji.com

[R66] 定时任务
来源：http://bhy.xinyue.icu

crontab -e;  crontab -l
来源：http://zbu.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://weh.jianghu66.top

openssl rand -hex 16
来源：http://cjt.sxryk.cn

[R68] 计算文件校验值
来源：http://quh.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://anc.mhx1999.top

[R69] 生成随机密码
来源：http://qot.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://kwb.tanke756.top

[R70] 时间戳与互转
来源：http://wmb.bjfxy.top

date +%s;  date -d @1700000000
来源：http://pqh.xziqi.cn

[R71] 日期格式化
来源：http://elm.chenjidiqi.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://ifw.jinqigufen.top

[R72] 等待端口就绪
来源：http://zal.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nfw.0kj1m.cn

[R73] 分割大日志
来源：http://gpp.yongpay.top

split -l 1000 big.log part_
来源：http://aev.uphjek.com

[R74] 批量重命名
来源：http://qyk.yj202588.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gbc.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://jlr.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://wgg.xinyue.icu

[R76] 使用临时文件
来源：http://gwd.9152youxi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rtf.mhx1999.top

[R77] 读取用户输入
来源：http://hni.yj202588.top

read -rp "请输入: " ans
来源：http://aez.yanxiufei.cn

[R78] 交互式菜单
来源：http://hmx.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uen.tarul.cn

[R79] 解析命令行选项
来源：http://vpn.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hyz.0kj1m.cn

[R80] 查看脚本执行耗时
来源：http://cyu.zhaomingkeji.xyz

time ./run.sh
来源：http://pfc.xinyue.icu

================================================================================
来源：http://syv.chenjidiqi.icu

S. C / C++ 专题
来源：http://yef.hysaishi.cn

================================================================================
来源：http://img.quarkkingdee.top

[S01] C：Hello World
来源：http://jnf.shanyushiyangtech.top

#include <stdio.h>
来源：http://mxt.daxiang520.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://iru.nanxuanxn.top

[S02] C：变量与格式化输出
来源：http://gvh.cheryme.top

int a = 10; printf("%d\n", a);
来源：http://tnt.0kj1m.cn

[S03] C：读入整数
来源：http://dxn.shangyingyoupin.top

int x; scanf("%d", &x);
来源：http://jbx.birdmap.top

[S04] C：字符串复制
来源：http://sef.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://ihx.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://kbj.daria6918.cn

strlen(s)
来源：http://zzk.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://osz.fehbvm.com

strcmp(a, b) == 0
来源：http://szf.gzhubu.top

[S07] C：数组遍历求和
来源：http://cms.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://etl.tanke756.top

[S08] C：动态内存分配与释放
来源：http://xbj.0kj1m.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nhv.yj20258.top

[S09] C：结构体定义与初始化
来源：http://nfj.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bjh.hesvh.cn

[S10] C：指针与解引用
来源：http://rmq.yfazqb.com

int *p = &a;  *p = 5;
来源：http://yfj.bbcook.cn

[S11] C：逐行读文件
来源：http://hdh.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://cda.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://szk.shzxlz.cn

fclose(f);
来源：http://lya.zhaomingkeji.xyz

[S12] C：写文件
来源：http://qkx.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ocr.shzxlz.cn

[S13] C：宏定义
来源：http://jiv.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://akj.jianghu66.top

[S14] C：枚举
来源：http://ppc.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://tdq.snrcjt.cn

[S15] C：类型转换
来源：http://kds.tian-w.cn

(double) a / b
来源：http://ktf.sufxvd.cn

[S16] C：位操作置位
来源：http://qje.daria6918.cn

x |= (1 << 3);
来源：http://nld.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://jjz.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pqf.shanyushiyangkeji.top

[S18] C：命令行参数
来源：http://iht.bbcook.cn

int main(int argc, char **argv)
来源：http://brf.cheryme.top

[S19] C：快速排序
来源：http://olv.dianchejie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zjp.feifeiyinyue.top

[S20] C：二分查找
来源：http://fby.yuxming.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hvc.ivvv.top

[S21] C：字符类别判断
来源：http://pzg.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pdn.zhoulong.xyz

[S22] C：字符串转数字
来源：http://vqq.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://dcw.zhixingplan.top

[S23] C：随机数
来源：http://eet.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://raf.gaohongyu789.top

[S24] C：获取本地时间
来源：http://qic.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aka.fzhhl.top

[S25] C：内存拷贝
来源：http://egv.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://fia.tanke756.top

[S26] C：内存清零
来源：http://vor.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://tkp.hnqzz.top

[S27] C：定义常量
来源：http://aha.svipenyu.cn

const double PI = 3.14159;
来源：http://xtk.zycfv.cn

[S28] C：静态变量
来源：http://uck.yfazqb.com

static int counter = 0;
来源：http://kbu.gogol.net.cn

[S29] C：变参函数
来源：http://eaw.fengsongda.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kxi.fzhhl.top

[S30] C：头文件保护
来源：http://jmw.fanxiaobao.xyz

#ifndef X_H
来源：http://vqm.svipenyu.cn

#define X_H
来源：http://cxq.birdmap.top

#endif
来源：http://vnv.chenjidiqi.icu

[S31] C++：Hello World
来源：http://psb.yj20258888.top

#include <iostream>
来源：http://oze.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://ilf.ybcxt.top

[S32] C++：字符串
来源：http://glb.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://xvc.hcnkem.com


<!-- 参考信息 -->