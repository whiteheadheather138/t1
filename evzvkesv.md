代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://esk.sjlbkw.cn

[Q52] 删除指定行
来源：http://xom.zhaomingkeji.xyz

DELETE FROM users WHERE id = 10;
来源：http://nkf.cdnleiting.top

[Q53] 按条件删除
来源：http://szr.nanxinkj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://joy.daxiang520.top

[Q54] 清空表
来源：http://wok.yueranfly.top

TRUNCATE TABLE logs;
来源：http://sqs.mhx1999.top

[Q55] 排名（并列占位）
来源：http://seh.hfpthk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ndc.tian-w.cn

[Q56] 密集排名（并列不占位）
来源：http://kmy.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rlj.dianchejie.cn

[Q57] 行号
来源：http://qbf.dianchejie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://otu.sufxvd.cn

[Q58] 累计求和
来源：http://qex.0kj1m.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://btm.9152youxi.cn

[Q59] 分组内累计
来源：http://shu.ybcxt.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://svl.jinqigfzy.top

[Q60] 取上一行 / 下一行
来源：http://bka.daria6918.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://esw.ydjk.org.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bis.chenzaomai.com

[Q61] 移动平均
来源：http://aqw.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vne.fzhhl.top

[Q62] 分组占比
来源：http://ssf.fanxiaobao.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dzr.daxiang520.top

[Q63] 开启事务
来源：http://cdy.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hpc.shuidangran.top

[Q64] 提交事务
来源：http://pij.zhaomingkeji.xyz

COMMIT;
来源：http://uyd.svipenyu.cn

[Q65] 回滚事务
来源：http://cqv.sxryk.cn

ROLLBACK;
来源：http://lpo.yuanzhike.top

[Q66] 行锁查询
来源：http://cxa.fktsv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gke.sweek.top

[Q67] 设置隔离级别
来源：http://irf.jlsjyb.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sta.sweek.top

[Q68] 保存点
来源：http://fik.shzxlz.cn

SAVEPOINT sp1;
来源：http://dov.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://fnl.ivvv.top

[Q69] 查看执行计划
来源：http://usj.hnqzz.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mpa.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://qnn.daria6918.cn

ANALYZE TABLE users;
来源：http://hrn.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://dqh.pengpengdd.cyou

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ccs.sufxvd.cn

[Q72] 查看索引
来源：http://jkg.nwbrower.top

SHOW INDEX FROM users;
来源：http://ynj.zhoulong.xyz

[Q73] 查看表状态
来源：http://eul.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://npt.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://quw.aibaodan.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ofh.chenlongwang.top

[Q75] 日期格式化
来源：http://nvi.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://okp.sxryk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bdk.quarkkingdee.top

[Q76] 按天统计
来源：http://hfa.ydjk.org.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jwc.aibaodan.cn

[Q77] 时间加减
来源：http://kkc.yuxming.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qzy.ppjwa.cn

[Q78] 当前时间
来源：http://mgf.jianghu66.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ddy.cucudq.cn

[Q79] 字符串拼接
来源：http://fgk.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yqt.zhixingplan.top

[Q80] 字符串截取
来源：http://tcj.yj20258.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://frz.xuanzx.com

[Q81] 字符串替换
来源：http://fzf.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nnb.zhiwuduotai.top

[Q82] 字符长度与字节长度
来源：http://xrf.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bvo.svipenyu.cn

[Q83] 大小写转换
来源：http://mvs.yuanzhike.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ngl.daxiang520.top

[Q84] 去除首尾空格
来源：http://tij.vehdjk.com

SELECT TRIM(name) FROM users;
来源：http://fau.iojbl.cn

[Q85] 数值取整
来源：http://abq.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uxz.hnqzz.top

[Q86] 读取 JSON 字段
来源：http://dly.pycfn.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fro.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://lfr.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wxm.zhijiandao.cn

[Q88] 行转列（条件聚合）
来源：http://hoy.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nml.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oeh.9152youxi.cn

[Q89] 判断表是否存在
来源：http://arl.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hie.sweek.top

[Q90] 生成序号列
来源：http://sul.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gxa.zhijiandao.cn

================================================================================
来源：http://qar.fengsongda.top

R. Bash 专题
来源：http://lza.dianchejie.cn

================================================================================
来源：http://zni.jinqigufen.top

[R01] shebang 与严格模式
来源：http://qka.yongpay.top

#!/usr/bin/env bash
来源：http://wqw.hywenlv.cn

set -euo pipefail
来源：http://lrf.guannengcc.top

[R02] 变量赋值与使用
来源：http://rrx.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://agu.smart0.xyz

[R03] 只读变量
来源：http://jng.bjfxy.top

readonly PI=3.14
来源：http://pfd.zhijiandao.cn

[R04] 位置参数
来源：http://mqo.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yta.ehwqpu.com

[R05] 参数默认值
来源：http://omr.cqqwz.cn

name="${1:-default}"
来源：http://msb.fengsongda.top

[R06] 判断命令是否存在
来源：http://bsz.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uhw.sjlbkw.cn

[R07] if 判断文件
来源：http://jtx.hongshengwenyu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lgf.jyoumei.cn

[R08] 数值比较
来源：http://dcn.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ynv.iojbl.cn

[R09] 字符串比较
来源：http://izu.hesvh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tjq.daxiang520.top

[R10] 正则匹配
来源：http://udp.tanke756.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gmz.zhoulong.xyz

[R11] case 多分支
来源：http://iif.fehbvm.com

case "$1" in
来源：http://bzq.ivvv.top

start) echo "启动" ;;
来源：http://bsf.cucudq.cn

stop)  echo "停止" ;;
来源：http://ras.ppjwa.cn

*)     echo "未知命令" ;;
来源：http://gun.yuxming.cn

esac
来源：http://jbi.yj202588.top

[R12] for 遍历文件
来源：http://gft.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://jyy.vqdsnc.cn

[R13] for 计数循环
来源：http://zhf.ywan-chungtsiang.top

for i in {1..10}; do echo "$i"; done
来源：http://lck.yongpay.top

[R14] C 风格 for
来源：http://bcf.jyoumei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kkc.birdmap.top

[R15] while 逐行读文件
来源：http://hwr.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wpi.chenjidiqi.icu

[R16] until 等待条件
来源：http://cbm.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jbh.jinyuanbaomall.cn

[R17] 数组定义与取值
来源：http://dyc.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://tzh.daxiang520.top

[R18] 遍历数组
来源：http://koe.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zjj.fengsongda.top

[R19] 数组长度
来源：http://oht.havefunace.top

echo "${#arr[@]}"
来源：http://sdh.nanxinkj.top

[R20] 关联数组（字典）
来源：http://piz.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ofn.tian-w.cn

[R21] 字符串长度
来源：http://jii.yvedp.cn

echo "${#s}"
来源：http://msu.xingfuxueyuan.xyz

[R22] 截取子串
来源：http://dxq.sysykeji.top

echo "${s:0:5}"
来源：http://uio.cqqwz.cn

[R23] 字符串替换
来源：http://laq.dashuyun.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jny.shuidangran.top

[R24] 大小写转换
来源：http://bxj.fanxiaobao.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://tqf.dianchejie.cn

[R25] 去后缀 / 去前缀
来源：http://emn.9152youxi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nam.jinyuanbaomall.cn

[R26] 命令替换
来源：http://lqw.chenlongwang.top

now=$(date +%F); echo "$now"
来源：http://ckt.zhongyouzk.top

[R27] 算术展开
来源：http://fpi.jinqigfzy.top

echo $((1 + 2 * 3))
来源：http://uol.yuanzhike.top

[R28] 浮点运算
来源：http://qxa.jlsjyb.cn

echo "scale=2; 10/3" | bc
来源：http://drc.sufxvd.cn

[R29] 定义函数
来源：http://cke.hnqzz.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://psi.52xcode.cn

[R30] 函数返回状态码
来源：http://wec.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://xll.vqdsnc.cn

[R31] 局部变量
来源：http://uce.fktsv.cn

f() { local x=1; echo "$x"; }
来源：http://omz.iojbl.cn

[R32] 参数个数校验
来源：http://fgr.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://okt.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://srk.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lba.iojbl.cn

[R34] 退出时清理
来源：http://cye.jqgfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://mlu.zhengqikj.top

[R35] 后台执行并等待
来源：http://dxe.hcnkem.com

sleep 5 & pid=$!; wait "$pid"
来源：http://wjl.yonumen.top

[R36] 并发执行多个任务
来源：http://hoj.zhiwuduotai.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kzv.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://vme.epnwcf.com

files=$(ls -1)
来源：http://gxs.zhixingplan.top

[R38] 管道串联
来源：http://fmh.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://pnk.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://gcr.meibo888.top

cmd > out.log 2>&1
来源：http://zae.316326.xyz

[R40] 追加写日志
来源：http://cxt.hesvh.cn

echo "log" >> out.log
来源：http://bus.iojbl.cn

[R41] 丢弃输出
来源：http://zpw.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://wbi.yuxming.cn

[R42] 输入重定向
来源：http://sed.sysykeji.top

wc -l < a.txt
来源：http://knh.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://lmw.gaohongyu789.top

find . -name "*.log" -type f
来源：http://zvt.jinghuilouyu.cn

[R44] 按修改时间查找
来源：http://pfr.pycfn.com

find . -mtime -7 -type f
来源：http://tck.cucudq.cn

[R45] 批量删除
来源：http://obs.sjlbkw.cn

find . -name "*.tmp" -delete
来源：http://buv.cheryme.top

[R46] 递归替换文件内容
来源：http://ppy.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ihc.yj20258.top

[R47] sed 单行替换
来源：http://hhv.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dsw.52xcode.cn

[R48] awk 取指定列
来源：http://rjn.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://ihr.xingfuxueyuan.xyz

[R49] awk 带条件
来源：http://dao.smart0.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wlm.andypj.xyz

[R50] awk 求和
来源：http://dga.yfazqb.com

awk '{s += $2} END {print s}' a.txt
来源：http://aqf.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://uqg.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nme.sufxvd.cn

[R52] 统计行数
来源：http://uzc.aibaodan.cn

wc -l a.txt
来源：http://jmk.yj20258.top

[R53] 查看文件头与实时尾
来源：http://wfd.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eji.hfpthk.cn

[R54] 比较两个文件
来源：http://nzt.jinyuanbaomall.cn

diff a.txt b.txt
来源：http://syl.shangyingyoupin.top

[R55] 压缩与解压
来源：http://swo.0kj1m.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jpa.nwbrower.top

[R56] 远程拷贝
来源：http://hww.ywan-chungtsiang.top

scp file user@host:/path/
来源：http://bkp.zdqjudy.top

[R57] 远程执行命令
来源：http://lnw.yangfankeji.com

ssh user@host 'uptime'
来源：http://emu.yuanzhike.top

[R58] 下载文件
来源：http://qzp.daxiang520.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wda.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://pkd.hfpthk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vdt.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://eti.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://buf.quarkkingdee.top

[R61] 磁盘占用
来源：http://jff.fehbvm.com

df -h;  du -sh *
来源：http://ywq.cheryme.top

[R62] 找最占空间的文件
来源：http://ayu.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://viz.yangfankeji.com

[R63] 内存与进程
来源：http://wge.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://nvr.jinqigufen.top

[R64] 结束进程
来源：http://pzi.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://add.zhixingplan.top

[R65] 查看端口占用
来源：http://yyk.316326.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ojc.svipenyu.cn

[R66] 定时任务
来源：http://kzb.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://jpk.yonumen.top

[R67] 生成随机十六进制串
来源：http://kwy.yuxming.cn

openssl rand -hex 16
来源：http://wri.ehwqpu.com

[R68] 计算文件校验值
来源：http://uzw.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://ghm.yongpay.top

[R69] 生成随机密码
来源：http://sal.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://wnc.c1oappe.top

[R70] 时间戳与互转
来源：http://jqc.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://ayx.jinqigfzy.top

[R71] 日期格式化
来源：http://hhs.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vvo.jinyuanbaomall.cn

[R72] 等待端口就绪
来源：http://jdq.guowangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wve.hnqzz.top

[R73] 分割大日志
来源：http://jxz.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://ppr.jinqigufen.top

[R74] 批量重命名
来源：http://zio.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nrs.cashguo.top

[R75] 导出环境变量
来源：http://mbe.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://yph.zdbjq.cn

[R76] 使用临时文件
来源：http://jep.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://taq.zhongyouzk.top

[R77] 读取用户输入
来源：http://akt.ppjwa.cn

read -rp "请输入: " ans
来源：http://dpy.yangfankeji.com

[R78] 交互式菜单
来源：http://kpi.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wja.cdnleiting.top

[R79] 解析命令行选项
来源：http://mad.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zdm.smart0.xyz

[R80] 查看脚本执行耗时
来源：http://cqp.quarkkingdee.top

time ./run.sh
来源：http://eya.nwbrower.top

================================================================================
来源：http://wsu.zhijiandao.cn

S. C / C++ 专题
来源：http://nib.redwolf501.top

================================================================================
来源：http://eks.wangdashe.top

[S01] C：Hello World
来源：http://wek.feifeiyinyue.top

#include <stdio.h>
来源：http://daz.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dlj.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://xtr.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://hvd.feifeiyinyue.top

[S03] C：读入整数
来源：http://dbc.bjfxy.top

int x; scanf("%d", &x);
来源：http://lhn.tianlin.xyz

[S04] C：字符串复制
来源：http://ntl.wangdashe.top

char dst[32]; strcpy(dst, "hi");
来源：http://kpe.aizwys.cn

[S05] C：字符串长度
来源：http://otd.jyoumei.cn

strlen(s)
来源：http://fmk.birdmap.top

[S06] C：字符串比较
来源：http://vlm.zhaomingkeji.xyz

strcmp(a, b) == 0
来源：http://pyo.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://xyo.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tuv.gogol.net.cn

[S08] C：动态内存分配与释放
来源：http://xgd.zhiwuduotai.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jvr.yangfankeji.com

[S09] C：结构体定义与初始化
来源：http://ccs.yangfankeji.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://egn.gotoacloud.top

[S10] C：指针与解引用
来源：http://dak.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://men.jianghu66.top

[S11] C：逐行读文件
来源：http://rgr.tarul.cn

FILE *f = fopen("a.txt", "r");
来源：http://boz.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://klw.yueranfly.top

fclose(f);
来源：http://iua.daxiang520.top

[S12] C：写文件
来源：http://sjq.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://axt.316326.xyz

[S13] C：宏定义
来源：http://xlh.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jtj.nanxuanxn.top

[S14] C：枚举
来源：http://taf.jianghu66.top

enum Color { RED, GREEN, BLUE };
来源：http://bla.jiagoushi.top

[S15] C：类型转换
来源：http://vfb.hesvh.cn

(double) a / b
来源：http://ghc.fehbvm.com

[S16] C：位操作置位
来源：http://hvg.xylfe.cn

x |= (1 << 3);
来源：http://mju.ctjpmb.com

[S17] C：安全拼接字符串
来源：http://otu.sjlbkw.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wjb.pengpengdd.cyou

[S18] C：命令行参数
来源：http://pce.fktsv.cn

int main(int argc, char **argv)
来源：http://auk.shangyingyoupin.top

[S19] C：快速排序
来源：http://ukv.guannengcc.top

qsort(a, n, sizeof(int), cmp);
来源：http://hjs.tianlin.xyz

[S20] C：二分查找
来源：http://mkl.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nuf.hfpthk.cn

[S21] C：字符类别判断
来源：http://ryx.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://goy.hnxiangtu.top

[S22] C：字符串转数字
来源：http://vrs.tianlin.xyz


<!-- 参考信息 -->