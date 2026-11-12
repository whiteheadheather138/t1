代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tkw.zhixingplan.top

[Q60] 取上一行 / 下一行
来源：http://fhm.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gir.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://teg.shanyushiyangtech.top

[Q61] 移动平均
来源：http://xej.ybcxt.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xxx.meibo888.top

[Q62] 分组占比
来源：http://ztj.hywenlv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lgr.pycfn.com

[Q63] 开启事务
来源：http://xzc.daxiang520.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vne.ydjk.org.cn

[Q64] 提交事务
来源：http://fdb.mhx1999.top

COMMIT;
来源：http://wpy.dianchejie.cn

[Q65] 回滚事务
来源：http://nrq.316326.xyz

ROLLBACK;
来源：http://ixz.9152youxi.cn

[Q66] 行锁查询
来源：http://wuu.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wch.ywan-chungtsiang.top

[Q67] 设置隔离级别
来源：http://sto.hongshengwenyu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lfb.cqqwz.cn

[Q68] 保存点
来源：http://euo.jianghu66.top

SAVEPOINT sp1;
来源：http://lcq.ydzc1.top

ROLLBACK TO sp1;
来源：http://nsg.shanyushiyangkeji.top

[Q69] 查看执行计划
来源：http://yed.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qri.guannengcc.top

[Q70] 更新统计信息
来源：http://hjy.fzhhl.top

ANALYZE TABLE users;
来源：http://jdk.fktsv.cn

[Q71] 查看建表语句
来源：http://jhy.kuanghao11.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tci.hnxiangtu.top

[Q72] 查看索引
来源：http://mjw.bjfxy.top

SHOW INDEX FROM users;
来源：http://hbi.hnxiangtu.top

[Q73] 查看表状态
来源：http://cuk.yonumen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://csg.jyoumei.cn

[Q74] 强制使用索引
来源：http://ins.gotoacloud.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wbi.aibaodan.cn

[Q75] 日期格式化
来源：http://mfb.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hkm.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rrs.nwbrower.top

[Q76] 按天统计
来源：http://qxd.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lir.zdqjudy.top

[Q77] 时间加减
来源：http://hdr.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://htw.jianghu66.top

[Q78] 当前时间
来源：http://mtf.dianchejie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ydg.sxryk.cn

[Q79] 字符串拼接
来源：http://haa.ydzc1.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eck.zycfv.cn

[Q80] 字符串截取
来源：http://jol.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ywe.gzhubu.top

[Q81] 字符串替换
来源：http://upu.snrcjt.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oue.sjlbkw.cn

[Q82] 字符长度与字节长度
来源：http://jll.redwolf501.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uvx.jiagoushi.top

[Q83] 大小写转换
来源：http://nig.shanyushiyangtech.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ywj.svipenyu.cn

[Q84] 去除首尾空格
来源：http://kxf.tanke756.top

SELECT TRIM(name) FROM users;
来源：http://tso.sjlbkw.cn

[Q85] 数值取整
来源：http://yzc.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gfd.wangshuangyany.cn

[Q86] 读取 JSON 字段
来源：http://jgy.nanxinkj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://neu.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://nhm.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kfd.sufxvd.cn

[Q88] 行转列（条件聚合）
来源：http://obp.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://edz.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xao.yanxiufei.cn

[Q89] 判断表是否存在
来源：http://hzl.iojbl.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fhu.xziqi.cn

[Q90] 生成序号列
来源：http://fbm.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hoz.cheryme.top

================================================================================
来源：http://dqo.zhoulong.xyz

R. Bash 专题
来源：http://mwj.chenjidiqi.icu

================================================================================
来源：http://atu.xuanzx.com

[R01] shebang 与严格模式
来源：http://jdb.daxiang520.top

#!/usr/bin/env bash
来源：http://nyi.hesvh.cn

set -euo pipefail
来源：http://als.guannengcc.top

[R02] 变量赋值与使用
来源：http://zuq.nwbrower.top

name="Tom"; echo "$name"
来源：http://pdw.hesvh.cn

[R03] 只读变量
来源：http://cwc.xylfe.cn

readonly PI=3.14
来源：http://coy.guannengcc.top

[R04] 位置参数
来源：http://nkv.birdmap.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xve.yj20258888.top

[R05] 参数默认值
来源：http://mys.ydzc1.top

name="${1:-default}"
来源：http://byp.jiagoushi.top

[R06] 判断命令是否存在
来源：http://huu.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bsi.dianchejie.cn

[R07] if 判断文件
来源：http://xem.yangfankeji.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oxl.nanxinkj.top

[R08] 数值比较
来源：http://nai.cheryme.top

if (( a > b )); then echo "a 更大"; fi
来源：http://txz.epnwcf.com

[R09] 字符串比较
来源：http://qya.9152youxi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mwq.kuanghao11.cn

[R10] 正则匹配
来源：http://ewz.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://moy.gotoacloud.top

[R11] case 多分支
来源：http://sfn.yj202588.top

case "$1" in
来源：http://mxw.cheryme.top

start) echo "启动" ;;
来源：http://buc.cheryme.top

stop)  echo "停止" ;;
来源：http://cst.hesvh.cn

*)     echo "未知命令" ;;
来源：http://ega.svipenyu.cn

esac
来源：http://tep.yanxiufei.cn

[R12] for 遍历文件
来源：http://xbe.andypj.xyz

for f in *.txt; do echo "$f"; done
来源：http://vvk.yangfankeji.com

[R13] for 计数循环
来源：http://klf.uphjek.com

for i in {1..10}; do echo "$i"; done
来源：http://rvc.ivvv.top

[R14] C 风格 for
来源：http://kup.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://soc.chenzaomai.com

[R15] while 逐行读文件
来源：http://zgx.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jrh.guannengcc.top

[R16] until 等待条件
来源：http://dah.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://flv.yvedp.cn

[R17] 数组定义与取值
来源：http://kxp.guowangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://nmi.0kj1m.cn

[R18] 遍历数组
来源：http://gvf.hnqzz.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://acf.snrcjt.cn

[R19] 数组长度
来源：http://hyz.hongshengwenyu.top

echo "${#arr[@]}"
来源：http://mqv.hcnkem.com

[R20] 关联数组（字典）
来源：http://dwv.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nbr.xinyue.icu

[R21] 字符串长度
来源：http://bfl.gzhubu.top

echo "${#s}"
来源：http://yft.jianghu66.top

[R22] 截取子串
来源：http://azk.cheryme.top

echo "${s:0:5}"
来源：http://jyh.sufxvd.cn

[R23] 字符串替换
来源：http://okf.cqqwz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fmw.jinqigfzy.top

[R24] 大小写转换
来源：http://yit.snrcjt.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mcz.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://kbj.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ksw.zdbjq.cn

[R26] 命令替换
来源：http://kpk.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://vkh.dashuyun.cn

[R27] 算术展开
来源：http://wly.zhijiandao.cn

echo $((1 + 2 * 3))
来源：http://gna.hongshengwenyu.top

[R28] 浮点运算
来源：http://wno.sufxvd.cn

echo "scale=2; 10/3" | bc
来源：http://wbn.316326.xyz

[R29] 定义函数
来源：http://puw.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://icy.gotoacloud.top

[R30] 函数返回状态码
来源：http://vbi.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://dtv.zhijiandao.cn

[R31] 局部变量
来源：http://yrg.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://ssm.316326.xyz

[R32] 参数个数校验
来源：http://ncj.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://drs.ivvv.top

[R33] 捕获错误并提示行号
来源：http://wex.quarkkingdee.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qej.yj20258888.top

[R34] 退出时清理
来源：http://xcl.guannengcc.top

trap 'rm -f "$tmp"' EXIT
来源：http://ngh.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://sjd.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ejm.shzxlz.cn

[R36] 并发执行多个任务
来源：http://uuj.tianlin.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ttb.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://vek.daxiang520.top

files=$(ls -1)
来源：http://zlc.nwbrower.top

[R38] 管道串联
来源：http://izn.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://wwz.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://huc.nwbrower.top

cmd > out.log 2>&1
来源：http://ffy.yj20258888.top

[R40] 追加写日志
来源：http://mfc.hywenlv.cn

echo "log" >> out.log
来源：http://xwg.shangyingyoupin.top

[R41] 丢弃输出
来源：http://rfi.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://lin.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://tsu.hnxiangtu.top

wc -l < a.txt
来源：http://wkv.xziqi.cn

[R43] 按名字查找文件
来源：http://ovj.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://cue.zhaomingkeji.xyz

[R44] 按修改时间查找
来源：http://foo.bbcook.cn

find . -mtime -7 -type f
来源：http://mkg.chenlongwang.top

[R45] 批量删除
来源：http://zph.sxryk.cn

find . -name "*.tmp" -delete
来源：http://qei.pycfn.com

[R46] 递归替换文件内容
来源：http://nui.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yre.xuetiantiany.cn

[R47] sed 单行替换
来源：http://qxv.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://bnr.yonumen.top

[R48] awk 取指定列
来源：http://cht.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://lsl.guannengcc.top

[R49] awk 带条件
来源：http://wza.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pto.haohaochexian.top

[R50] awk 求和
来源：http://tyu.pycfn.com

awk '{s += $2} END {print s}' a.txt
来源：http://zae.guannengcc.top

[R51] 排序去重取前几
来源：http://vur.hammf.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fhu.guannengcc.top

[R52] 统计行数
来源：http://cxf.hnqzz.top

wc -l a.txt
来源：http://bzd.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://bys.jinyuanbaomall.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nmr.snrcjt.cn

[R54] 比较两个文件
来源：http://slv.mhx1999.top

diff a.txt b.txt
来源：http://kqe.redwolf501.top

[R55] 压缩与解压
来源：http://kmg.jlsjyb.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tau.jyoumei.cn

[R56] 远程拷贝
来源：http://xut.jianghu66.top

scp file user@host:/path/
来源：http://ygc.svipenyu.cn

[R57] 远程执行命令
来源：http://aio.sxryk.cn

ssh user@host 'uptime'
来源：http://fij.shuidangran.top

[R58] 下载文件
来源：http://jvy.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fxx.smart0.xyz

[R59] 发 POST JSON
来源：http://lqq.hywenlv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ewl.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://rpn.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dyg.aibaodan.cn

[R61] 磁盘占用
来源：http://xwc.yonumen.top

df -h;  du -sh *
来源：http://tcb.feifeiyinyue.top

[R62] 找最占空间的文件
来源：http://xsy.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://xne.guowangkeji.top

[R63] 内存与进程
来源：http://etm.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://aqg.nanxinkj.top

[R64] 结束进程
来源：http://ler.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://xfc.c1oappe.top

[R65] 查看端口占用
来源：http://rck.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pfo.birdmap.top

[R66] 定时任务
来源：http://uer.aibaodan.cn

crontab -e;  crontab -l
来源：http://ntl.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://vqf.xuanzx.com

openssl rand -hex 16
来源：http://aag.hongshengwenyu.top

[R68] 计算文件校验值
来源：http://ocq.jlsjyb.cn

sha256sum a.txt;  md5sum a.txt
来源：http://upr.haohaochexian.top

[R69] 生成随机密码
来源：http://lrj.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://qju.zdqjudy.top

[R70] 时间戳与互转
来源：http://mdx.hcnkem.com

date +%s;  date -d @1700000000
来源：http://dxc.316326.xyz

[R71] 日期格式化
来源：http://pxv.nwbrower.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lkt.ydzc1.top

[R72] 等待端口就绪
来源：http://xis.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fsy.andypj.xyz

[R73] 分割大日志
来源：http://vfs.quarkkingdee.top

split -l 1000 big.log part_
来源：http://oyf.zdbjq.cn

[R74] 批量重命名
来源：http://ygd.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tbb.smart0.xyz

[R75] 导出环境变量
来源：http://jer.sweek.top

export PATH="$HOME/bin:$PATH"
来源：http://pdn.svipenyu.cn

[R76] 使用临时文件
来源：http://wny.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tbu.yueranfly.top

[R77] 读取用户输入
来源：http://vwp.hysaishi.cn

read -rp "请输入: " ans
来源：http://raq.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://bul.bjfxy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tlr.guowangkeji.top

[R79] 解析命令行选项
来源：http://jav.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://agv.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://qis.mhx1999.top

time ./run.sh
来源：http://bfl.fanxiaobao.xyz

================================================================================
来源：http://wfj.hongshengwenyu.top

S. C / C++ 专题
来源：http://ivo.ybcxt.top

================================================================================
来源：http://vga.hfpthk.cn

[S01] C：Hello World
来源：http://vim.ywan-chungtsiang.top

#include <stdio.h>
来源：http://fpt.xinyue.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://swu.tanke756.top

[S02] C：变量与格式化输出
来源：http://rfi.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://wnd.tian-w.cn

[S03] C：读入整数
来源：http://pkx.hesvh.cn

int x; scanf("%d", &x);
来源：http://psg.gaohongyu789.top

[S04] C：字符串复制
来源：http://yvm.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://twe.nanxinkj.top

[S05] C：字符串长度
来源：http://atf.shzxlz.cn

strlen(s)
来源：http://onb.tanke756.top

[S06] C：字符串比较
来源：http://ijd.vehdjk.com

strcmp(a, b) == 0
来源：http://dwu.wangshuangyany.cn

[S07] C：数组遍历求和
来源：http://xco.daxiang520.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zqd.fengsongda.top

[S08] C：动态内存分配与释放
来源：http://gon.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tbv.ydjk.org.cn

[S09] C：结构体定义与初始化
来源：http://mui.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://syp.quarkkingdee.top

[S10] C：指针与解引用
来源：http://myk.c1oappe.top

int *p = &a;  *p = 5;
来源：http://xqt.kuanghao11.cn

[S11] C：逐行读文件
来源：http://jkf.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://szk.aizwys.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nsc.yueranfly.top

fclose(f);
来源：http://vdv.xuetiantiany.cn

[S12] C：写文件
来源：http://srw.dashuyun.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hzv.jqgufenzy.top

[S13] C：宏定义
来源：http://nie.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oei.316326.xyz

[S14] C：枚举
来源：http://pbg.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://lxa.fktsv.cn

[S15] C：类型转换
来源：http://cji.jqgufenzy.top

(double) a / b
来源：http://jwx.xylfe.cn

[S16] C：位操作置位
来源：http://cww.birdmap.top

x |= (1 << 3);
来源：http://dyn.yueranfly.top

[S17] C：安全拼接字符串
来源：http://pkf.xziqi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tdu.yangfankeji.com

[S18] C：命令行参数
来源：http://vvz.gogol.net.cn

int main(int argc, char **argv)
来源：http://ois.daria6918.cn

[S19] C：快速排序
来源：http://txf.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://lcn.yj202588.top

[S20] C：二分查找
来源：http://yof.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ved.mhx1999.top

[S21] C：字符类别判断
来源：http://vnu.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gbi.pycfn.com

[S22] C：字符串转数字
来源：http://cmf.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jhb.wangdashe.top

[S23] C：随机数
来源：http://uzt.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mlv.xylfe.cn

[S24] C：获取本地时间
来源：http://yko.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pxt.aibaodan.cn

[S25] C：内存拷贝
来源：http://pkz.sufxvd.cn

memcpy(dst, src, n);
来源：http://sra.yj202588.top

[S26] C：内存清零
来源：http://nur.ybcxt.top

memset(a, 0, sizeof a);
来源：http://ezb.zdqjudy.top

[S27] C：定义常量
来源：http://pqs.c1oappe.top

const double PI = 3.14159;
来源：http://rzx.redwolf501.top

[S28] C：静态变量
来源：http://wqn.xinyue.icu

static int counter = 0;
来源：http://wfh.xuetiantiany.cn

[S29] C：变参函数
来源：http://bjc.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cwy.aizwys.cn

[S30] C：头文件保护
来源：http://aar.shanyushiyangtech.top


<!-- 参考信息 -->